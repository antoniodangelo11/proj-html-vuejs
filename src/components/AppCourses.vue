<script></script>

<template>
    <section class="bg_courses">
        <div class="courses container">
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
                                <h5 class="fw-bold">Pass Plus</h5>
                                <button class="btn_learn fw-bold">LEARN MORE</button>
                            </div>
                        </div>
                        <div>
                            <img src="../assets/img/course-intensive-200x200.jpg" alt="">
                            <div class="py-3">
                                <h5 class="fw-bold">Intensive Course</h5>
                                <button class="btn_learn fw-bold">LEARN MORE</button>
                            </div>
                        </div>
                        <div>
                            <img src="../assets/img/courses-instructor-200x200.jpg" alt="">
                            <div class="py-3">
                                <h5 class="fw-bold">Instructors</h5>
                                <button class="btn_learn fw-bold">LEARN MORE</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_courses {
    background-image: url(../assets/img/promise-background.jpg);
    background-size: cover;
    background-position-y: 500px;

    .courses {
        max-width: 1000px;
    }

    .course_info {
        box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.6);
        position: relative;
        bottom: 1.5rem;
        background-color: rgb(255, 255, 255);

        h2 {
            color: #494C4E;
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
            border: 0px solid #000000;
            background-color: #7ABC64;
            color: #FFFFFF;
            transition: transform 0.3s ease-in-out;

            &:hover {
                transform: scale(1.05);
            }
        }
    }

    .learn_more {
        .btn_learn {
            border-radius: 100px;
            border: 3px solid #929aa3;
            background-color: transparent;
            color: #929aa3;
            padding: 10px 20px;
            transition: transform 0.3s ease-in-out;

            &:hover {
                transform: scale(1.05);
                color: #7ABC64;
            }
        }

        h5 {
            color: #929aa3;
        }
    }
}
</style>