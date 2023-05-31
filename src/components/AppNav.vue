<script>
export default {
    props: {
        ObjNav: Object,
    },
};
</script>

<template>
    <li class="fw-bold">
        {{ ObjNav.title }}
        <span class="btn text-light rounded fw-bold">{{ ObjNav.sub_title }}</span>
    </li>
</template>

<style lang="scss" scoped>
li {
    color: rgb(255, 255, 255);

    &:hover {
        color: #7ABC64;
        cursor: pointer;
        border-bottom: 2px solid #7ABC64;
    }

    span {
        display: none;
    }

    &:nth-child(4) span {
        display: inline-block;
        background-color: #7ABC64;
        padding: .1rem;
        margin-bottom: .4rem;
        font-size: .6em;
    }
}
</style>