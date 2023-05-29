<script>
export default {

}
</script>

<template>
    <main>
        <section class="user_registration container">
            <div class="row">
                <div class="col-6">
                    <div class="text_sign_in p-4">
                        <h3 class="py-2 fw-bold">Get Behind The Wheel</h3>
                        <p class="py-2">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rerum magnam quasi
                            impedit
                            aliquam
                            dolor
                            saepe vel, minus inventore tenetur tempore alias nihil odio quia nisi placeat quisquam ullam
                            deserunt dolores!</p>
                        <p class="py-2">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam, quis ipsum.
                            Quibusdam ipsum
                            maiores
                            tempora cumque facere accusantium, deleniti assumenda? Similique laudantium odit, qui
                            aperiam ab
                            modi cumque consectetur excepturi.
                            Est tempore doloribus atque.
                        </p>
                    </div>
                </div>

                <div class="col-6">
                    <div class="form_sign_in p-5 rounded">
                        <h2 class="text-center py-3">First Lesson Free!</h2>
                        <p class="text-center py-3">Whenyou make a block booking with us your first lesson is included
                            free.</p>
                        <div class="input-group mb-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default" placeholder="Your Name*">
                            <span class="input-group-text"><img src="../assets/img/image.png" alt=""></span>
                        </div>
                        <div class="input-group mb-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default" placeholder="Email*">
                        </div>
                        <div class="input-group mb-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default" placeholder="Telephone*">
                        </div>
                        <div class="input-group mb-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default" placeholder="Location*">
                        </div>
                        <div class="text-center">
                            <button class="btn_green fw-bold p-2">REQUEST A CALLBACK</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="bg_call_us">
            <div class="call_us container d-flex align-items-center justify-content-between py-5">
                <div class="text-light">
                    <h3>Start Learning to Drive Today</h3>
                    <p>Give us a call to schedule your first driving lesson</p>
                </div>
                <div class="text-light">
                    <font-awesome-icon class="px-2 text-light" :icon="['fas', 'phone']" flip="horizontal" />
                    1-800-555-555
                </div>
            </div>
        </section>

        <section class="bg_courses container">
            <div class="courses_container d-flex">
                <div class="row">
                    <div class="col-4">
                        <div class="course_info p-5 rounded">
                            <h2 class="text-center py-2 fw-bold">Courses</h2>
                            <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum, eius.
                                Perferendis vero
                                officia
                                asperiores? Cum harum voluptatem libero sapiente nemo, beatae mollitia ad ipsum nulla venia.
                            </p>
                            <div class="text-center py-2">
                                <button class="btn_green fw-bold p-2">COURSE INFORMATION</button>
                            </div>
                            <img src="../assets/img/new-corner.jpg" alt="">
                        </div>
                    </div>

                    <div class="col-8">
                        <div class="learn_more d-flex align-items-center gap-4 py-5 text-center">
                            <div>
                                <img src="../assets/img/courses-passplus-200x200.jpg" alt="">
                                <div class="py-3">
                                    <h4 class="fw-bold">Pass Plus</h4>
                                    <button class="btn_learn fw-bold">LEARN MORE</button>
                                </div>
                            </div>
                            <div>
                                <img src="../assets/img/course-intensive-200x200.jpg" alt="">
                                <div class="py-3">
                                    <h4 class="fw-bold">Pass Plus</h4>
                                    <button class="btn_learn fw-bold">LEARN MORE</button>
                                </div>
                            </div>
                            <div>
                                <img src="../assets/img/courses-instructor-200x200.jpg" alt="">
                                <div class="py-3">
                                    <h4 class="fw-bold">Pass Plus</h4>
                                    <button class="btn_learn fw-bold">LEARN MORE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section>

        </section>
    </main>
</template>

<style lang="scss" scoped>
.user_registration {
    max-width: 1000px;

    .form_sign_in {
        -moz-box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        position: relative;
        bottom: 2.5rem;
        background-color: white;
    }

    h2 {
        color: #7ABC64;
    }

    h3 {
        color: #494C4E;
    }

    p {
        color: #929aa3;
    }

    .btn_green {
        border-radius: 100px 100px 100px 100px;
        -moz-border-radius: 100px 100px 100px 100px;
        -webkit-border-radius: 100px 100px 100px 100px;
        border: 0px solid #000000;
        background-color: #7ABC64;
        color: #FFFFFF;
    }
}

.bg_call_us {
    background-image: url(../assets/img/horizontal-cta-background.jpg);
    background-size: cover;
    background-position: center;

    .call_us {
        max-width: 1000px;
    }
}

.bg_courses {
    max-width: 1000px;

    .course_info {
        -moz-box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        position: relative;
        bottom: 1.5rem;
        background-color: white;

        h2 {
            color: #7ABC64;
        }

        p {
            color: #929aa3;
        }

        img {
            width: 50px;
            position: absolute;
            top: 0;
            left: 0;
            border-radius: 5px 0px 0px 0px;
        }

        .btn_green {
            border-radius: 100px 100px 100px 100px;
            -moz-border-radius: 100px 100px 100px 100px;
            -webkit-border-radius: 100px 100px 100px 100px;
            border: 0px solid #000000;
            background-color: #7ABC64;
            color: #FFFFFF;
        }
    }

    .learn_more {
        .btn_learn {
            border-radius: 100px;
            border: 3px solid #929aa3;
            background-color: transparent;
            color: #929aa3;
            padding: 10px 20px;
        }

        h4 {
            color: #929aa3;
        }
    }
}
</style>