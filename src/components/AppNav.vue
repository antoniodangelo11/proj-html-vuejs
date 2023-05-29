<script>
export default {
    props: {
        ObjNav: Object,
    },
};
</script>

<template>
    <li class="fw-bold text-light">
        {{ ObjNav.title }}
    </li>
</template>

<style lang="scss" scoped></style>