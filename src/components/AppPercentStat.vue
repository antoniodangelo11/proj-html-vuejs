<script>
export default {
    props: {
        DataPercent: Array,
    },
};
</script>

<template>
    <section class="bg_svg py-5">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="percent_drivers d-flex py-3 gap-2">
                        <div v-for="percent in this.DataPercent" :key="percent.title" class="percent_info rounded p-5">
                            <img :src="percent.img" :alt="percent.img">
                            <div class="percent fs-1">{{ percent.percent }}</div>
                            <p class="text-center fw-bold">{{ percent.title }}</p>
                        </div>
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
        box-shadow: -7px 11px 29px -7px rgba(133, 133, 133, 0.6);
        position: relative;
        background-color: rgb(255, 255, 255);
        border-top: 7px solid #7ABC64;

        .percent {
            position: absolute;
            bottom: 0;
            right: 50%;
            top: 50%;
            color: #929aa3;
            transform: translate(60%, -35%);
        }

        p {
            color: #929aa3;
            padding-top: 2rem;
        }
    }
}
</style>