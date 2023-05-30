<script>
export default {
    props: {
        DataInstructors: Array,
    },

};
</script>

<template>
    <section class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-7">
                    <div class="d-flex flex-column">
                        <h2>Your Instructors</h2>
                        <p class="py-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto ipsam
                            laborum cupiditate
                            accusantium
                            mollitia odit quasi distinctio nemo impedit ullam vitae.
                        </p>
                    </div>
                </div>
                <div class="col-5">
                    <div class="d-flex justify-content-center flex-column">
                        <button class="btn_green fw-bold align-self-end">MORE ABOUT US</button>
                    </div>
                </div>
            </div>

            <div class="row">
                <div class="col-12">
                    <div class="instructor_info d-flex gap-4 py-3">
                        <div v-for="instructor in this.DataInstructors" :key="instructor.name"
                            class="card_instructors p-5 rounded d-flex flex-column text-center">

                            <img :src="instructor.img" :alt="instructor.img">
                            <h5 class="py-3 fw-bold">{{ instructor.name }}</h5>
                            <div class="icons_social">
                                <i class="fa-brands fa-facebook px-2"></i>
                                <i class="fa-brands fa-twitter px-2"></i>
                                <i class="fa-brands fa-instagram px-2"></i>
                            </div>
                            <p class="py-2">{{ instructor.text }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.container {
    max-width: 1000px;
    margin: auto;

    .info_instructors {
        h2 {
            color: #494C4E;
        }

        p {
            color: #929aa3;
        }
    }
}

.col-5 {
    padding: 4.5rem 0 0 1.5rem;

    .btn_green {
        border-radius: 100px 100px 100px 100px;
        border: 0px solid #000000;
        background-color: #7ABC64;
        color: #FFFFFF;
        padding: .5rem 8rem;
        white-space: nowrap;
    }
}

.instructor_info> :nth-child(2) {
    transform: scale(1.1);
}

.card_instructors {
    box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.6);
    position: relative;
    background-color: rgb(255, 255, 255);
    border-top: 7px solid #7ABC64;
    margin-top: 2rem;

    h5 {
        color: #494C4E;
    }

    p {
        color: #929aa3;
    }

    .icons_social {
        i {
            color: #929aa3;
        }
    }
}
</style>