<script>
import AppRegistration from './AppRegistration.vue';
import AppCallUs from './AppCallUs.vue';
import AppCourses from './AppCourses.vue';
import AppPercentStat from './AppPercentStat.vue';

export default {
    data() {
        return {
            ArrPercent: [
                {
                    img: 'src/assets/img/95.png',
                    title: 'PASS RATE',
                },
                {
                    img: 'src/assets/img/100.png',
                    title: 'REFERRAL RATE',
                },
                {
                    img: 'src/assets/img/0.png',
                    title: 'ACCIDENT RATE',
                },
            ],
        }
    },
    components: {
        AppRegistration,
        AppCallUs,
        AppCourses,
        AppPercentStat,
    },
};
</script>

<template>
    <main>
        <AppRegistration />
        <AppCallUs />
        <AppCourses />
        <AppPercentStat :DataPercent="this.ArrPercent" />
    </main>
</template>

<style lang="scss" scoped></style>