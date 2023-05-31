<script>
export default {
    props: {
        DataNews: Array,
    },
};
</script>

<template>
    <section class="bg_news">
        <div class="container">
            <div class="row">
                <div class="col-10 offset-1">
                    <div class="news_content">
                        <div class="news_card d-flex flex-column align-items-center rounded-top">
                            <h2 class="fw-bold">Latest News</h2>
                            <div class="d-flex">
                                <div v-for="news in this.DataNews" :key="news.title" class="px-3">
                                    <div class="img_container">
                                        <img class="w-100" :src="news.img" :alt="news.img">
                                    </div>
                                    <div class="text_card text-center">
                                        <div class="title py-2 fs-4 fw-bold">{{ news.title }}</div>
                                        <small class="sub_title">{{ news.sub_title }}</small>
                                        <div class="text py-2">{{ news.text }}</div>
                                    </div>
                                </div>
                            </div>
                            <button class="btn_green fw-bold">MORE FROM THE BLOG</button>
                        </div>
                        <img class="news_triangle" src="../assets/img/latestnews-bottom-1200x105.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_news {
    background-image: url(../assets/img/latestnews-background.jpg);
    background-size: cover;
    background-position: bottom;
}

.news_content {
    max-width: 1000px;
    margin: auto;
    padding-bottom: 4rem;
}

.news_card {
    box-shadow: -7px 11px -1px -7px rgba(133, 133, 133, 0.6);
    background-color: rgb(255, 255, 255);
    border-top: 7px solid #929aa3;
    margin-top: 2rem;
    padding: 3rem;
    position: relative;
    margin-top: -3rem;

    h2 {
        color: #494C4E;
        margin-bottom: 2rem;
    }

    .title {
        color: #7ABC64;
    }

    .sub_title {
        color: #929aa3;
    }

    .text {
        color: #929aa3;
    }
}

.img_container {
    img {
        transition: transform 0.3s ease-in-out;

        &:hover {
            transform: scale(1.05);
        }
    }
}

.btn_green {
    border-radius: 100px 100px 100px 100px;
    border: 0px solid #000000;
    background-color: #7ABC64;
    color: #FFFFFF;
    padding: .5rem 2rem;
    white-space: nowrap;
    margin-top: 3rem;

    transition: transform 0.3s ease-in-out;

    &:hover {
        transform: scale(1.05);
    }
}

.news_triangle {
    width: 1000px;
}
</style>