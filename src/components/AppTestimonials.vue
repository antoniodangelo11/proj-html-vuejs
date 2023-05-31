<script>
export default {

    props: {
        DataTestimonials: Array,
    },
};
</script>
<template>
    <section class="testimonials">
        <div class="container">
            <div class="row">
                <div class="col-10 offset-1">
                    <div class="carousel-item active">
                        <div v-for="testimonial in DataTestimonials" :key="testimonial.name"
                            class="testimonial_card d-flex flex-column text-center">
                            <div class="title">
                                <h2 class="fw-bold">{{ testimonial.title }}</h2>
                                <p>{{ testimonial.sub_title }}</p>
                            </div>
                            <div class="img_container">
                                <img :src="testimonial.img" :alt="testimonial.img">
                            </div>
                            <div class="name_info">
                                <p>{{ testimonial.text }}</p>
                                <h4>{{ testimonial.name }}</h4>
                            </div>
                            <div class="icons_circle py-2">
                                <i class="fa-solid fa-circle fa-2xs px-1"></i>
                                <i class="fa-regular fa-circle fa-2xs px-1"></i>
                                <i class="fa-regular fa-circle fa-2xs px-1"></i>
                                <i class="fa-regular fa-circle fa-2xs px-1"></i>
                                <i class="fa-regular fa-circle fa-2xs px-1"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.testimonials {
    background-image: url(../assets/img/testimonial-background.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    margin-top: -5rem;
    height: 650px;
}

.container {
    max-width: 1000px;
    margin: auto;
}

.testimonial_card {
    margin-top: 8rem;
}

.title {
    h2 {
        color: #494C4E;
    }

    p {
        color: #929aa3;
        font-size: 1.5rem;
    }
}

.name_info {
    p {
        color: #929aa3;
    }

    h4 {
        color: #494C4E;
    }
}

.icons_circle {
    i {
        color: #929aa3;
    }

}


.img_container {
    width: 120px;
    margin: auto;

    img {
        width: 100%;
    }
}
</style>