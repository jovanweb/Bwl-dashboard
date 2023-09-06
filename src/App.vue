<template>
  <main>
    <FirstStepPDF v-if="step === 1" @previewData="preview"/>
    <FinalPDF v-if="step === 2" :dataUser="dataUser"/>
  </main>
    
</template>
<script>
import html2pdf from 'html2pdf.js';
import FirstStepPDF from './components/FirstStepPDF.vue';
import FinalPDF from './components/FinalPDF.vue';

export default {
  name: 'App',
  components: {
    FirstStepPDF, FinalPDF,
  },
  data() {
    return {
      dataUser: null,
      step:1,
    }
  },
  methods: {
    generatePDF() {
      const content = this.$refs.pdfContent;
      const pdfOptions = {
        margin: 10,
        filename: 'example.pdf',
        image: { type: 'jpeg', quality: 0.98 },
        html2canvas: { scale: 2 },
        jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' },
      };

      html2pdf().from(content).set(pdfOptions).save();
    },

    preview(preview) {
      this.dataUser = preview;
      this.step = 2;
    }
  },
}

</script>
<style lang="scss">

  html, body, #app {
    height: 100%;
    font-family: 'Roboto', sans-serif;
  }

  p, .form-check-label {
    color: #555555;
  }
</style>

<style lang="scss" scoped>

  main {
    height: 100%;
  }
  #pdf-content {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    padding: 20px;
  }

  .title {
    font-size: 24px;
    color: #333;
  }

  .content {
    font-size: 16px;
    color: #555;
  }
</style>
