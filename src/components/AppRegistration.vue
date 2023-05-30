<script>
export default {

}
</script>

<template>
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
</style>