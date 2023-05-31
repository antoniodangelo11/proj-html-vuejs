<script>
import AppNav from './AppNav.vue';

export default {
    data() {
        return {
            ArrNav: [
                {
                    title: 'HOME',
                    link: '#',
                    id: 0,
                },
                {
                    title: 'ABOUT',
                    link: '#',
                    id: 1,
                },
                {
                    title: 'PRICES',
                    link: '#',
                    id: 2,
                },
                {
                    title: 'COURSES',
                    sub_title: 'NEW',
                    link: '#',
                    id: 3,
                },
                {
                    title: 'LOCATIONS',
                    link: '#',
                    id: 4,
                },
                {
                    title: 'BLOG',
                    link: '#',
                    id: 5,
                },
            ],
        };
    },
    components: {
        AppNav,
    },
};
</script>

<template>
    <header>
        <div class="top_nav_bg" id="start">
            <div class="top_nav container d-flex justify-content-between align-items-center">
                <small>We have a 95% Successful Pass Rate!</small>
                <small>
                    <font-awesome-icon class="px-2" :icon="['fas', 'phone']" flip="horizontal" />Give us a call to book
                    your
                    tuituon!
                    1-800-555-555
                </small>
            </div>
        </div>
        <div class="nav_cover">
            <div class="nav_bg">
                <div class="navbar container d-flex">
                    <img class="d-block" src="../assets/img/avada-drivers-logo-2x-200x39.png" alt="">
                    <ul class="list-unstyled d-flex">
                        <AppNav v-for="ObjNav in ArrNav" :key="ObjNav.id" :ObjNav="ObjNav" />
                    </ul>
                    <div>
                        <button class="btn_green fw-bold p-2">BOOK NOW</button>
                    </div>
                </div>
            </div>
            <div class="title_text container text-light fw-bold d-flex flex-column justify-content-center">
                <h1>Drive with Avada</h1>
                <p>We Offer the finest driving tuition money can buy</p>
            </div>
        </div>
        <div class="cart_fixed">
            <div class="py-2">
                <i class="fa-solid fa-cart-shopping fa-flip-horizontal fa-xs"></i>
            </div>
        </div>
        <div class="folder_fixed">
            <div class="py-2">
                <i class="fa-regular fa-folder-open fa-xs"></i>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.top_nav_bg {
    background-color: rgb(28, 29, 30);

    .top_nav {
        max-width: 1000px;
        height: 3rem;
        color: rgb(146, 154, 163);
    }
}

.nav_cover {
    background-image: url(../assets/img/homepage-hero-background.jpg);
    background-size: cover;
    background-position: center;
    height: 600px;

    .nav_bg {
        background-color: rgba(73, 76, 78, .5);
    }

    .btn_green {
        border-radius: 100px 100px 100px 100px;
        border: 0px solid #000000;
        background-color: #7ABC64;
        color: #FFFFFF;
        transition: transform 0.3s ease-in-out;

        &:hover {
            transform: scale(1.05);
        }
    }

    .navbar {
        max-width: 1000px;
        height: 6rem;
        padding: none;
        align-items: first baseline;

        img {
            position: relative;
            top: 10px;
        }

        ul {
            gap: 2.5rem;
        }
    }

    .title_text {
        max-width: 1000px;
        height: 100%;

    }
}

.cart_fixed {
    background-color: #f6f6f6;
    padding: .2rem 1rem;
    position: fixed;
    top: 18.5%;
    right: 1%;
    border-radius: 5px 5px 5px 5px;
    cursor: pointer;
}

.folder_fixed {
    background-color: #f6f6f6;
    padding: .2rem 1rem;
    position: fixed;
    top: 13%;
    right: 1%;
    border-radius: 5px 5px 5px 5px;
    cursor: pointer;
}
</style>