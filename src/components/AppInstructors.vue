<script>
export default {
    props: {
        DataInstructors: Array,
    },

};
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-7">
                    <div class="info_instructors d-flex flex-column">
                        <h2>Your Instructors</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto ipsam
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
                    <div class="d-flex gap-3 py-3">
                        <div v-for="instructor in this.DataInstructors" :key="instructor.name"
                            class="card_instructors p-5 rounded">
                            <img :src="instructor.img" :alt="instructor.img">
                            <h5>{{ instructor.name }}</h5>
                            <div>
                                <span><i class="fa-brands fa-facebook"></i></span>
                                <span><i class="fa-brands fa-twitter"></i></span>
                                <span><i class="fa-brands fa-instagram"></i></span>
                            </div>
                            <p>{{ instructor.text }}</p>
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
    padding: 3rem 0 0 1.5rem;
}

.btn_green {
    border-radius: 100px 100px 100px 100px;
    -moz-border-radius: 100px 100px 100px 100px;
    -webkit-border-radius: 100px 100px 100px 100px;
    border: 0px solid #000000;
    background-color: #7ABC64;
    color: #FFFFFF;
    padding: .5rem 5rem;
    white-space: nowrap;
}

.card_instructors {
    -moz-box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
    box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
    position: relative;
    background-color: rgb(255, 255, 255);
    border-top: 7px solid #7ABC64;
    margin-top: 2rem;
}
</style>