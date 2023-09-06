
<template>
    <div class="container">
        <section class="first-step">
            <aside class="aside">
                <div class="upload-image-wrapper">
                    <input ref="photo" @change="setPhoto" type="file" id="upload-photo">
                    <label class="upload-image" for="upload-photo" :style="'background-image: url(' + dataUser.source + ')'">
                        <svg v-if="!dataUser.source" xmlns="http://www.w3.org/2000/svg" width="40" viewBox="0 0 24 24"><path fill="#222" d="M19 13a1 1 0 0 0-1 1v.38l-1.48-1.48a2.79 2.79 0 0 0-3.93 0l-.7.7-2.48-2.48a2.85 2.85 0 0 0-3.93 0L4 12.6V7a1 1 0 0 1 1-1h7a1 1 0 0 0 0-2H5a3 3 0 0 0-3 3v12a3 3 0 0 0 3 3h12a3 3 0 0 0 3-3v-5a1 1 0 0 0-1-1ZM5 20a1 1 0 0 1-1-1v-3.57l2.9-2.9a.79.79 0 0 1 1.09 0l3.17 3.17 4.3 4.3Zm13-1a.89.89 0 0 1-.18.53L13.31 15l.7-.7a.77.77 0 0 1 1.1 0L18 17.21Zm4.71-14.71-3-3a1 1 0 0 0-.33-.21 1 1 0 0 0-.76 0 1 1 0 0 0-.33.21l-3 3a1 1 0 0 0 1.42 1.42L18 4.41V10a1 1 0 0 0 2 0V4.41l1.29 1.3a1 1 0 0 0 1.42 0 1 1 0 0 0 0-1.42Z"/></svg>
                    </label>
                </div>

                <input type="text" id="name" name="name" class="form-control form-control-sm mb-2" placeholder="Full Name" v-model="dataUser.userName">
                <input type="text" id="name" name="name" class="form-control form-control-sm mb-5" placeholder="Position" v-model="dataUser.position">

                <h3><strong>CONTACT</strong></h3>
                <ul class="list-unstyled">
                    <li class="d-flex align-items-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="me-2" width="15" viewBox="0 0 10 12" fill="none"><path fill="#39A6DE" d="M3.407.61c.019-.011.014-.018.081.014.068.032.175.115.28.229.21.23.421.578.531.808l.012.021c.31.534.443.942.447 1.198.005.257-.064.367-.281.492l-.563.324c-.367.21-.54.589-.582.94-.044.353.02.696.178.967l1.387 2.39c.158.271.424.498.752.637.329.14.744.179 1.11-.032l.563-.322c.218-.125.348-.129.57.003.22.132.508.45.818.983a3.716 3.716 0 0 1 .451.883c.048.148.066.282.06.356-.006.074-.008.066-.027.078l-.427.245c-1.074.466-2.058.361-2.938-.096-.883-.457-1.65-1.286-2.184-2.258l-.004-.005-1.17-2.016c0-.003-.002-.004-.003-.007-.578-.946-.917-2.021-.875-3.01.042-.986.444-1.887 1.388-2.58L3.407.61Zm.342-.537c-.185-.086-.44-.111-.648.009l-.452.26L2.62.36C1.532 1.156 1.03 2.265.982 3.408c-.05 1.142.332 2.321.962 3.352l1.164 2.004h.002l.001.006c.582 1.055 1.417 1.97 2.434 2.499a3.936 3.936 0 0 0 3.503.097l.452-.26a.71.71 0 0 0 .33-.553 1.499 1.499 0 0 0-.085-.593 4.054 4.054 0 0 0-.51-1.01c-.335-.572-.655-.97-1.027-1.192a1.172 1.172 0 0 0-1.192-.01l-.563.323c-.166.096-.36.086-.563 0a1.088 1.088 0 0 1-.463-.381L4.04 5.299c-.07-.121-.127-.37-.1-.589.026-.219.114-.39.28-.486l.562-.323c.367-.21.596-.596.589-1.03-.008-.432-.194-.91-.528-1.486a4.084 4.084 0 0 0-.621-.941 1.522 1.522 0 0 0-.473-.37Z"/></svg>
                        <input type="text" id="name" name="name" class="form-control form-control-sm" placeholder="Phone" v-model="dataUser.phone">
                    </li>
                    <li class="d-flex align-items-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="me-2" width="15" viewBox="0 0 12 9" fill="none"><path fill="#39A6DE" d="m.556 1.17 4.428 3.295a.282.282 0 0 0 .333 0L9.744 1.17v4.812c0 .09-.086.184-.24.184H.796c-.154 0-.24-.094-.24-.184V1.17Zm.24-.616h8.707c.044 0 .081.008.113.02a.251.251 0 0 0-.027.02L5.15 3.898.712.594A.221.221 0 0 0 .684.576.298.298 0 0 1 .797.554Zm0-.554C.377 0 0 .318 0 .74v5.242c0 .422.375.738.797.738h8.706c.422 0 .799-.316.799-.738V.74c0-.422-.377-.74-.799-.74H.797Z"/><path fill="#39A6DE" d="M10.153 1.457a.277.277 0 1 0 0 .554h.757c.17 0 .263.103.263.192v5.312c0 .09-.093.193-.263.193H1.825c-.17 0-.263-.104-.263-.193v-.844a.278.278 0 1 0-.556 0v.844c0 .431.39.747.82.747h9.084c.43 0 .82-.316.82-.747V2.203c0-.43-.39-.746-.82-.746h-.757Z"/></svg>
                        <input type="text" id="name" name="name" class="form-control form-control-sm" placeholder="Email" v-model="dataUser.email">
                    </li>
                    <li class="d-flex align-items-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="me-2" width="15" viewBox="0 0 12 12" fill="none"><path fill="#39A6DE" d="M3.189 6.436h2.334v4.508a6.8 6.8 0 0 1-2.334-4.508Zm-2.545 0h1.94a7.394 7.394 0 0 0 1.915 4.35 5.153 5.153 0 0 1-3.197-2.395 5.19 5.19 0 0 1-.658-1.955ZM4.5.8a7.39 7.39 0 0 0-1.946 5.035H.605a5.165 5.165 0 0 1 .7-2.639A5.15 5.15 0 0 1 4.5.8ZM5.523.644v5.191H3.157v-.038A6.794 6.794 0 0 1 5.521.644ZM5.824 0c-.009 0-.017 0-.025.002A5.83 5.83 0 0 0 .78 2.897a5.77 5.77 0 0 0 0 5.794 5.831 5.831 0 0 0 5.023 2.895l.021.001a5.838 5.838 0 0 0 4.43-2.032.298.298 0 0 0-.024-.435.302.302 0 0 0-.434.046 5.226 5.226 0 0 1-2.68 1.658 7.407 7.407 0 0 0 1.169-1.648c.17-.351-.347-.617-.536-.276a6.823 6.823 0 0 1-1.623 2.04V6.437h.663a.302.302 0 0 0 .303-.3.3.3 0 0 0-.303-.3h-.663V.625a6.807 6.807 0 0 1 1.88 2.593.301.301 0 1 0 .559-.227A7.42 7.42 0 0 0 7.146.772a5.207 5.207 0 0 1 3.557 3.172.302.302 0 1 0 .563-.213A5.826 5.826 0 0 0 5.825 0Z"/><path fill="#39A6DE" d="M8.528 4.333a.19.19 0 0 1 .084.024l2.397 1.398-.923.191a.3.3 0 0 0-.198.445l.661 1.141c.031.054.016.109-.037.14l-.44.253c-.055.03-.111.016-.142-.038L9.268 6.75a.302.302 0 0 0-.486-.05l-.625.695L8.14 4.63c-.001-.074.056-.166.168-.23.003 0 .003-.002.005-.003l.01-.005a.39.39 0 0 1 .205-.058Zm.033-.6c-.494 0-1.014.39-1.025.9l.018 2.778c.002.267.077.511.3.637.224.126.502.026.65-.137l.45-.504.454.78c.193.334.63.45.965.258l.44-.254a.705.705 0 0 0 .26-.959l-.455-.782.668-.137c.217-.045.443-.235.444-.49.002-.255-.172-.443-.404-.578L8.917 3.839v.002a.71.71 0 0 0-.356-.107Z"/></svg>
                        <input type="text" id="name" name="name" class="form-control form-control-sm" placeholder="Website" v-model="dataUser.website">
                    </li>
                    <li class="d-flex align-items-center mb-5">
                        <svg xmlns="http://www.w3.org/2000/svg" class="me-2" width="15" viewBox="0 0 11 12" fill="none"><path fill="#39A6DE" d="M5.865.582a3.048 3.048 0 0 1 3.057 3.04c0 .652-.28 1.642-.874 2.33L5.865 8.48 3.682 5.953c-.594-.689-.874-1.679-.874-2.332 0-1.678 1.37-3.039 3.057-3.039Zm0-.582c-2.005 0-3.64 1.627-3.64 3.621 0 .807.304 1.887 1.013 2.71L4.256 7.51H2.507a.293.293 0 0 0-.277.201L.992 11.52a.29.29 0 0 0 .278.38h9.19a.29.29 0 0 0 .278-.38L9.5 7.71a.292.292 0 0 0-.278-.2H8.11c-.41-.02-.41.602 0 .58h.899l1.048 3.227H1.673L2.72 8.091h2.038l.783.907h-.514a.283.283 0 1 0 0 .565h1.674c.159.003.29-.125.29-.283a.283.283 0 0 0-.29-.282h-.512L8.49 6.33a4.335 4.335 0 0 0 1.015-2.71C9.506 1.627 7.87 0 5.865 0Z"/><path fill="#39A6DE" d="M6.493 4.246a.888.888 0 0 1-1.256-1.25.888.888 0 0 1 1.256 0c.35.348.35.902 0 1.25Zm.414.411a1.465 1.465 0 0 0 0-2.072 1.484 1.484 0 0 0-2.083 0 1.463 1.463 0 0 0 0 2.072c.572.57 1.51.57 2.083 0Z"/></svg>
                        <input type="text" id="name" name="name" class="form-control form-control-sm" placeholder="Location" v-model="dataUser.location">
                    </li>
                </ul>

                <h3><strong>PROFESSIONAL SKILLS</strong></h3>
                <ul class="list-unstyled">
                    <li v-for="skill in dataUser.skills" :key="skill.id">
                        <div class="form-check">
                            <input class="form-check-input" type="checkbox" v-model="skill.checked" :id="skill.name" />
                            <label class="form-check-label" :for="skill.name">{{skill.name}}</label>
                        </div>
                    </li>
                </ul>
            </aside>
            <article class="content">
                <h3><strong>WORK EXPERIENCE</strong></h3>
                <div class="current-position d-flex mb-3 gap-2">
                    <input type="text" placeholder="Position in BWL" class="form-control form-control-sm w-50" v-model="dataUser.positionInBWL">
                    <input type="text" placeholder="From - Present" class="form-control form-control-sm w-50" v-model="dataUser.time">
                </div>
                <ul class="list-unstyled project-list">
                    <li v-for="project in dataUser.projects" :key="project.id">
                        <div class="checkblock">
                            <input type="checkbox" :id="project.id" v-model="project.checked">
                            <label :for="project.id">
                                <h3><strong>{{project.name}}</strong></h3>
                                <p class="mb-0">{{project.description}}</p>
                            </label>
                        </div>
                    </li>
                </ul>

                <div class="previous-jobs">
                    <h3><strong>PREVIOUS WORK EXPERIENCE</strong></h3>

                    <ul class="list-unstyled" v-if="dataUser.jobs">
                        <li v-for="(job,index) in dataUser.jobs" :key="index" class="d-flex gap-3">
                            <svg xmlns="http://www.w3.org/2000/svg" width="46" height="46" viewBox="0 0 25 25" fill="none"><path fill="#39A6DE" d="M0 0h25v25H0z"/><path fill="#fff" d="M6.25 10.447a.352.352 0 0 0 0 .673l4.124 1.278 7.071-5.345.04-.053L6.25 10.447ZM10.386 13.27l-.53 1.422a.35.35 0 0 0 .452.452l1.423-.53 4.16-5.506-5.505 4.162ZM17.947 7.555l-5.345 7.071 1.278 4.124a.352.352 0 0 0 .673 0L18 7.516l-.053.04ZM8.872 14.14a.351.351 0 0 0-.497 0l-2.11 2.109a.351.351 0 1 0 .498.497l2.109-2.11a.351.351 0 0 0 0-.496ZM10.86 16.128a.351.351 0 0 0-.497 0l-2.109 2.11a.351.351 0 1 0 .497.497l2.11-2.11a.351.351 0 0 0 0-.497ZM9.061 15.939a.351.351 0 0 0-.497 0l-2.461 2.46a.351.351 0 1 0 .497.498l2.461-2.46a.351.351 0 0 0 0-.498Z"/></svg>
                            <div>
                                <h3 class="mb-0"><strong>{{job.jobPosition}}</strong> at {{job.jobCompany}}</h3>
                                <p class=" mb-0">{{job.jobDate}}</p>
                            </div>

                            <a href="javascript:;" class="remove-job text-danger" @click="removeJob(index)">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="feather feather-x"><path d="M18 6 6 18M6 6l12 12"/></svg>
                            </a>
                        </li>
                    </ul>
                    <div class="d-flex gap-2 flex-wrap">
                        <div class="flex-grow-1">
                            <input type="text" class="form-control flex-1 form-control-sm" placeholder="Job Position" v-model="addJobPosition">
                        </div>
                        <div class="flex-grow-1">
                            <input type="text" class="form-control flex-1 form-control-sm" placeholder="Company" v-model="addJobCompany">
                        </div>
                        <div class="flex-grow-1">
                            <input type="text" class="form-control flex-1 form-control-sm" placeholder="Time From - To" v-model="addJobDate">
                        </div>
                        <div class="flex-grow-1">
                            <button class="btn btn-primary btn-sm w-100" @click="addNewJob">Add job</button>
                        </div>
                    </div>
                </div>

                <div class="education">
                    <h3><strong>EDUCATION</strong></h3>

                    <ul class="list-unstyled" v-if="dataUser.education">
                        <li v-for="(edu,index) in dataUser.education" :key="index" class="d-flex gap-3">
                            <svg xmlns="http://www.w3.org/2000/svg" width="46" height="46" viewBox="0 0 25 25" fill="none"><path fill="#39A6DE" d="M0 0h25v25H0z"/><path fill="#FBFBFB" d="M12.516 16.267c2.489 0 5.134-.817 5.134-2.333v-2.296l-4.642 1.74a1.413 1.413 0 0 1-.98.001L7.35 11.637v2.297c0 1.516 2.676 2.333 5.165 2.333Z"/><path fill="#FBFBFB" d="m20.182 8.828-7.498-2.8a.518.518 0 0 0-.336 0L4.924 8.8h7.592a.467.467 0 0 1 0 .934H4.551v9.8a.466.466 0 0 0 .93.063l.028.085a.466.466 0 1 0 .885-.295l-.91-2.728v-6.71l6.864 2.557a.527.527 0 0 0 .336 0l7.498-2.8a.468.468 0 0 0 .3-.44.468.468 0 0 0-.3-.438Z"/></svg>
                            <div>
                                <h3 class="mb-0"><strong>{{edu.educationUniversity}}</strong></h3>
                                <p class=" mb-0">{{edu.gradeLevel}}</p>
                            </div>

                            <a href="javascript:;" class="remove-education text-danger" @click="removeEducation(index)">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="feather feather-x"><path d="M18 6 6 18M6 6l12 12"/></svg>
                            </a>
                        </li>
                    </ul>
                    <div class="d-flex gap-2 flex-wrap">
                        <div class="flex-grow-1">
                            <input type="text" class="form-control flex-1 form-control-sm" placeholder="University, City" v-model="addUniversity">
                        </div>
                        <div class="flex-grow-1">
                            <input type="text" class="form-control flex-1 form-control-sm" placeholder="Grade Level" v-model="addGradeLevel">
                        </div>
                        <div class="flex-grow-1">
                            <button class="btn btn-primary btn-sm w-100" @click="addNewEducation">Add Education</button>
                        </div>
                    </div>
                </div>
            </article>
        </section>
        <section class="footer p-3">
            <button class="btn btn-success" @click="preview">Preview</button>
        </section>
    </div>
</template>
<script>

export default {
    name:"FirstStepPDF",
    emits: ['previewData'],
    data() {
        return {
            dataUser: {
                source: null,
                userName: "",
                position: "",
                phone: "",
                email: "",
                website: "",
                location: "",
                positionInBWL: "",
                time: "",
                skills: [
                    {
                        id: 1,
                        name: "Swift",
                        checked: true,
                    },
                    {
                        id: 2,
                        name: "Objective C",
                        checked: true,
                    },
                    {
                        id: 3,
                        name: "Kotlin",
                        checked: true,
                    },
                    {
                        id: 4,
                        name: "Git/SVN",
                        checked: true,
                    },
                    {
                        id: 5,
                        name: "HTML & CSS",
                        checked: true,
                    },
                    {
                        id: 6,
                        name: "Java",
                        checked: true,
                    },
                    {
                        id: 7,
                        name: "PHP",
                        checked: false,
                    },
                ],
                projects: [
                    {
                        id: 1,
                        name: "Sentry Sync",
                        description: "SentrySync is the ultimate external USB add-on accessory for your Tesla vehicle with the ability to sync dashcam and sentry videos directly to your mobile device. All footage is analyzed using our cutting edge artificial intelligence to provide additional insights such as facial and license plate recognition.",
                        checked: false,
                    },
                    {
                        id: 2,
                        name: "Aspen Properties",
                        description: "An all-encompassing service request, tenant communication, room bookings and mobile door access solution, specifically branded to your company. Perfect for office, residential, and retail.",
                        checked: true,
                    },
                    {
                        id: 3,
                        name: "GeoInspect",
                        description: "Create digital inspections for your sites that can only be completed when entering the geofence of that property for full integrity.Site Managers and Site Inspectors can easily complete various digital inspections with a few easy clicks that gets submitted into a digital catalogue for easy future retrieval and sorting.",
                        checked: true,
                    },
                    {
                        id: 4,
                        name: "HotButton",
                        description: "Productivity app. Worked in a cross functional team to investigate, help define and implement key functionality. Implemented all of in-app recording which is unique to the Android version of the app. Provided code reviews and mentoring for another developer on the team. Wrote integration tests.",
                        checked: false,
                    },
                    {
                        id: 5,
                        name: "FLD",
                        description: "Digitally transform paper-driven business processes into the digital version.",
                        checked: true,
                    },
                    {
                        id: 6,
                        name: "Dating Apps",
                        description: "Various dating apps smilar to Tinder in features and funcionality.",
                        checked: true,
                    },
                    {
                        id: 7,
                        name: "AppAranger/ HA",
                        description: "System for Booking all kind of services on the territory of Switzerland and Germany",
                        checked: false,
                    },
                ],
                jobs: [],
                education: [],
            },
            addJobPosition: "",
            addJobCompany: "",
            addJobDate: "",

            addUniversity: "",
            addGradeLevel: "",
        }
    },
    methods: {

        addNewJob() {
            this.dataUser.jobs.push(
                {
                    jobPosition: this.addJobPosition,
                    jobCompany: this.addJobCompany,
                    jobDate: this.addJobDate,
                }
            )

            this.addJobPosition= "";
            this.addJobCompany= "";
            this.addJobDate= "";
        },

        addNewEducation() {
            this.dataUser.education.push(
                {
                    educationUniversity: this.addUniversity,
                    gradeLevel: this.addGradeLevel,
                }
            )

            this.addUniversity= "";
            this.addGradeLevel= "";
        },
        
        removeJob(index) {
            this.dataUser.jobs.splice(index,1)
        },
        removeEducation(index) {
            this.dataUser.education.splice(index,1)
        },
        async setPhoto($event) {
            if (!$event.target.files.length) {
                return;
            }
            
            const [file] = $event.target.files;
            this.type = file.type;
            
            const reader = new FileReader();
            reader.readAsDataURL(file);
            
            await new Promise((resolve) => {
                reader.onloadend = () => {
                this.dataUser.source = reader.result;
                resolve(); // Resolve the Promise when done
                };
            });
        },

        preview() {
            this.$emit('previewData', this.dataUser)
        }
    },
}
</script>
<style lang="scss" scoped>

    .container {
        max-width: 1024px;
    }

    .upload-image-wrapper {
        input {
            visibility: hidden;
            opacity: 0;
            position: absolute;
            z-index: -1;
        }
    }

    .upload-image {
        width: 200px;
        aspect-ratio: 1 / 1;
        border: 1px solid #bababa;
        margin-bottom: 20px;
        cursor: pointer;
        background-size: cover;
        background-position: 50% 50%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .first-step {
        display: flex;
        border-radius: 2px;
        margin-top: 30px;
        border: 1px solid #bababa;
    }

    h3 {
        font-size: 16px;
        color: #39A6DE;
    }
    .aside {
        width: 40%;
        padding: 20px;
    }
    .content {
        background-color: #FBFBFB;
        width: 60%;
        padding: 20px;
    }

    .project-list {
        overflow: auto;
        max-height: 500px;

        li:not(:last-child) {
            margin-bottom: 10px;
        }
    }

    .checkblock {
        
        input {
            visibility: hidden;
            opacity: 0;
            position: absolute;
            z-index: -1;
        }

        label {
            border: 1px solid #222222;
            border-radius: 5px;
            padding: 15px;
            display: block;
            transition: all .3s ease;
            cursor: pointer;
        }

        input:checked + label {
            background-color: rgba(#39A6DE, .2);
            border-color: #39A6DE; 
        }

        p {
            font-size: 14px;
        }
    }
    
    .previous-jobs {
        border-top: 1px solid #222;
        padding-top: 15px;

        li {
            position: relative;
            border-bottom: 1px solid #bababa;
            padding: 10px;

            .remove-job {
                position: absolute;
                right: 0;
                top: 50%;
                transform: translate(0,-50%);
                
            }

            h3 {
                color: #555555;
            }

            p {
                font-size: 16px;
            }
        }
    }

    .education {
        border-top: 1px solid #222;
        padding-top: 15px;
        margin-top: 20px;

        li {
            position: relative;
            border-bottom: 1px solid #bababa;
            padding: 10px;

            .remove-education {
                position: absolute;
                right: 0;
                top: 50%;
                transform: translate(0,-50%);
                
            }

            h3 {
                color: #555555;
            }

            p {
                font-size: 16px;
            }
        }
    }

    .footer {
        border: 1px solid #bababa;
        border-top: 0;
        margin-bottom: 50px;
        display: flex;
        flex-direction: row-reverse;
    }
</style>