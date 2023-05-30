<script>
import AppRegistration from './AppRegistration.vue';
import AppCallUs from './AppCallUs.vue';
import AppCourses from './AppCourses.vue';
import AppPercentStat from './AppPercentStat.vue';
import AppInstructors from './AppInstructors.vue';
import AppTestimonials from './AppTestimonials.vue';
import AppLatestNews from './AppLatestNews.vue';

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
            ArrTestimonials: [
                {
                    title: 'Testimonials',
                    sub_title: `Here's what our happy drivers had to say about our services:`,
                    img: 'src/assets/img/testimonial-sophia.png',
                    text: 'Avada Driving School reall helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Higly recommended.',
                    name: 'Sophia Jones',
                },
                {
                    title: 'Testimonials',
                    sub_title: `Here's what our happy drivers had to say about our services:`,
                    img: 'src/assets/img/testimonial-grant.png',
                    text: 'Avada Driving School reall helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Higly recommended.',
                    name: 'Grant Harvey',
                },
                {
                    title: 'Testimonials',
                    sub_title: `Here's what our happy drivers had to say about our services:`,
                    img: 'src/assets/img/testimonial-kelly.png',
                    text: 'Avada Driving School reall helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Higly recommended.',
                    name: 'Kelly Johnson',
                },
                {
                    title: 'Testimonials',
                    sub_title: `Here's what our happy drivers had to say about our services:`,
                    img: 'src/assets/img/testimonial-harold.png',
                    text: 'Avada Driving School reall helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Higly recommended.',
                    name: 'Harold Green',
                },
                {
                    title: 'Testimonials',
                    sub_title: `Here's what our happy drivers had to say about our services:`,
                    img: 'src/assets/img/testimonial-kate.png',
                    text: 'Avada Driving School reall helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Higly recommended.',
                    name: 'Kate Lewis',
                },
            ],
            ArrNews: [
                {
                    img: 'src/assets/img/blog-choosecar-700x441.jpg',
                    title: 'What Car to Start With?',
                    sub_title: 'February 7th 2019 | 0 Comments',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing'
                },
                {
                    img: 'src/assets/img/blogpost-10and2-700x441.jpg',
                    title: 'Avada Driving School Expanding',
                    sub_title: 'February 7th 2019 | 0 Comments',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing'
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
        AppTestimonials,
        AppLatestNews,
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
        <AppTestimonials :DataTestimonials="this.ArrTestimonials" />
        <AppLatestNews :DataNews="this.ArrNews" />
    </main>
</template>

<style lang="scss" scoped></style>