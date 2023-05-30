<script>
export default {
    props: {
        DataPercent: Array,
    },
};
</script>

<template>
    <section class="bg_svg">
        <div class="container">
            <div class="col-4">
                <div class="percent_drivers d-flex gap-3 py-3">
                    <div v-for="percent in this.DataPercent" :key="percent.title" class="percent_info p-5 rounded">
                        <img :src="percent.img" :alt="percent.img">
                        <p class="text-center fw-bold">{{ percent.title }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_svg {
    background-image: url(../assets/svg/driving-triangle.svg);
    background-size: cover;
}

.container {
    max-width: 1000px;

    .percent_info {
        -moz-box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.4);
        position: relative;
        background-color: rgb(255, 255, 255);
        border-top: 7px solid #7ABC64;
        ;

        p {
            color: #929aa3;
            padding-top: 2rem;
        }
    }
}
</style>