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
                        <div class="input-group mb-3">
                            <input type="text" class="form-control bg-body-tertiary" aria-label="Sizing example input"
                                aria-describedby="inputGroup-sizing-default">
                        </div>
                        <button class="btn_green fw-bold w-100">MORE FROM THE BLOG</button>
                        <div class="sub_title text-center">(We do not share your data with anybody, and only use it for
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
}

.sub_title {
    font-size: .8em;
}
</style>