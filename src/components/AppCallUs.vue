<script>
export default {

}
</script>

<template>
    <section class="bg_call_us">
        <div class="row">
            <div class="col-12">
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
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_call_us {
    background-image: url(../assets/img/horizontal-cta-background.jpg);
    background-size: cover;
    background-position: center;

    .call_us {
        max-width: 1000px;
    }
}
</style>