<script>
export default {

}
</script>

<template>
    <section class="bg_contact">
        <div class="container">
            <div class="row">
                <div class="col-3">
                    <div class="text_info py-3">
                        <img src="../assets/img/avada-drivers-logo-2x-200x39.png" alt="">
                        <div class="text">Avada Driving School is the right choice for experienced drivers looking for a
                            refresher
                            course, or the brand new driver wanting to pass first time.
                        </div>
                    </div>
                </div>
                <div class="col-3">
                    <ul class="contact_details">
                        <li class="fw-bold text-light py-3">CONTACT DETAILS</li>
                        <li>
                            <i class="fa-solid fa-house"></i>
                            12345 North Main Street, New York, NY 555555
                        </li>
                        <li>
                            <i class="fa-solid fa-phone fa-flip-horizontal"></i>
                            1.800.555.6789
                        </li>
                        <li>
                            <i class="fa-regular fa-envelope"></i>
                            info@your-domain.com
                        </li>
                        <li>
                            <i class="fa-solid fa-link"></i>
                            Theme-Fusion.com
                        </li>
                    </ul>
                </div>
                <div class="col-3">
                    <ul class="courses_details">
                        <li class="fw-bold text-light py-3">COURSES</li>
                        <li>
                            <i class="fa-solid fa-circle-arrow-right"></i>
                            Pass Plus
                        </li>
                        <li>
                            <i class="fa-solid fa-circle-arrow-right"></i>
                            Intensive Course
                        </li>
                        <li>
                            <i class="fa-solid fa-circle-arrow-right"></i>
                            Automatic
                        </li>
                        <li>
                            <i class="fa-solid fa-circle-arrow-right"></i>
                            Instructor Training
                        </li>
                    </ul>
                </div>
                <div class="col-3">
                    <div class="img_footer py-3">
                        <img class="px-1" src="../assets/img/labels-400x87TOP.png" alt="">
                        <img src="../assets/img/labels-400x87BOT.png" alt="">
                    </div>
                    <div>
                        <button class="btn_green fw-bold p-3">BOOK NOW</button>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_contact {
    background-image: url(../assets/img/footer-background-color.jpg);
    background-position: center;
}

.container {
    max-width: 1000px;
    padding-top: 3rem;
    padding-bottom: 3rem;
}

.text_info {
    .text {
        color: #929aa3;
        font-size: .9em;
        padding-top: .5rem;
    }
}

.btn_green {
    border-radius: 100px 100px 100px 100px;
    border: 0px solid #000000;
    background-color: #7ABC64;
    color: #FFFFFF;
    margin-top: 1rem;
    margin-left: 2.6rem;
}

.contact_details {
    list-style: none;

    i,
    li {
        color: #929aa3;
    }

    li {
        font-size: .9em;
        padding-bottom: 1rem;
    }
}

.courses_details {
    list-style: none;
    color: #7ABC64;

    li {
        font-size: .9em;
        padding-bottom: 1rem;
    }
}
</style>