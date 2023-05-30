<script>
import AppRegistration from './AppRegistration.vue';
import AppCallUs from './AppCallUs.vue';
import AppCourses from './AppCourses.vue';
import AppPercentStat from './AppPercentStat.vue';
import AppInstructors from './AppInstructors.vue';

export default {
    data() {
        return {
            ArrPercent: [
                {
                    img: 'src/assets/img/95.png',
                    percent: '95%',
                    title: 'PASS RATE',
                },
                {
                    img: 'src/assets/img/100.png',
                    percent: '100%',
                    title: 'REFERRAL RATE',
                },
                {
                    img: 'src/assets/img/0.png',
                    percent: '0%',
                    title: 'ACCIDENT RATE',
                },
            ],
            ArrInstructors: [
                {
                    img: 'src/assets/img/instructor-mikehart-200x127.jpg',
                    name: 'Mike Hart',
                    text: 'Lorem ipsum dolor si amet, consectetur adispiscing elit.',
                },
                {
                    img: 'src/assets/img/instructor-johnsmith-200x127.jpg',
                    name: 'John Smith',
                    text: 'Lorem ipsum dolor si amet, consectetur adispiscing elit.',
                },
                {
                    img: 'src/assets/img/instructor-angelahart-200x127.jpg',
                    name: 'Angela Hart',
                    text: 'Lorem ipsum dolor si amet, consectetur adispiscing elit.',
                },
            ],
        }
    },
    components: {
        AppRegistration,
        AppCallUs,
        AppCourses,
        AppPercentStat,
        AppInstructors,
    },
};
</script>

<template>
    <main>
        <AppRegistration />
        <AppCallUs />
        <AppCourses />
        <AppPercentStat :DataPercent="this.ArrPercent" />
        <AppInstructors :DataInstructors="this.ArrInstructors" />
    </main>
</template>

<style lang="scss" scoped></style>