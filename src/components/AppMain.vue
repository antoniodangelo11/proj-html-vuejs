<script>
import AppRegistration from './AppRegistration.vue';
import AppCallUs from './AppCallUs.vue';
import AppCourses from './AppCourses.vue';
import AppPercentStat from './AppPercentStat.vue';

export default {
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
        <AppPercentStat />
    </main>
</template>

<style lang="scss" scoped></style>