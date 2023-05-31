<script>
export default {

}
</script>

<template>
    <section class="bg_newsletter">
        <div class="container">
            <div class="row">
                <div class="col-10 offset-1">
                    <div class="newsletter_content">
                        <h2 class="text-center">Sign up to our Newsletter</h2>
                        <div class="input-group mb-3 py-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default">
                        </div>
                        <button class="btn_green fw-bold w-100">MORE FROM THE BLOG</button>
                        <div class="sub_title text-center py-3">(We do not share your data with anybody, and only use it for
                            its intended
                            purpose)</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_newsletter {
    background-image: url(../assets/img/newsletter_background.jpg);
    background-size: cover;
}

.newsletter_content {
    max-width: 500px;
    margin: auto;
    padding-top: 3rem;
    padding-bottom: 3rem;

    h2 {
        color: #494C4E;
    }
}

.btn_green {
    border-radius: 100px 100px 100px 100px;
    border: 0px solid #000000;
    background-color: #7ABC64;
    color: #FFFFFF;
    padding: .5rem 2rem;
    white-space: nowrap;
}

.sub_title {
    font-size: .7em;
    color: #929aa3;

}
</style>