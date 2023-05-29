<script>
export default {

}
</script>

<template>
    <header>
        <div class="top_nav_bg">
            <div class="top_nav container d-flex justify-content-between align-items-center">
                <small>We have a 95% Successful Pass Rate!</small>
                <small>
                    <font-awesome-icon class="px-2" :icon="['fas', 'phone']" />Give us a call to book your
                    tuituon!
                    1-800-555-555
                </small>
            </div>
        </div>
        <div class="nav_cover">
            <div class="nav_bg">
                <nav class="navbar">
                    <img src="../assets/img/avada-drivers-logo-2x-200x39.png" alt="">
                </nav>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.top_nav_bg {
    background-color: rgb(73, 76, 78);

    .top_nav {
        height: 3rem;
        color: rgb(146, 154, 163);
    }
}

.nav_cover {
    background-image: url(../assets/img/homepage-hero-background.jpg);
    background-size: cover;
    height: 600px;
}

.nav_bg {
    background-color: rgba(73, 76, 78, .5);
}
</style>