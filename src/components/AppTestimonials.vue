<script>
export default {
    data() {
        return {
            activeIndex: 0,
            isAutorun: true,
            sliderDirection: 1,
            idAutorun: null,
            autorunTime: 3000,
        }
    },
    // methods: {
    //     methods: {
    //         prevSlide() {
    //             this.activeIndex--;
    //             if (this.activeIndex < 0) {
    //                 this.activeIndex = this.arrImages.length - 1;
    //             }
    //         },

    //         nextSlide() {
    //             this.activeIndex++;
    //             if (this.activeIndex >= this.arrImages.length) {
    //                 this.activeIndex = 0;
    //             }
    //         },

    //         clickActiveImg(index) {
    //             this.activeIndex = index;
    //         },

    //         runSlider() {
    //             if (this.isAutorun) {
    //                 this.idAutorun = setInterval(
    //                     () => this.sliderDirection == 1 ? this.nextSlide() : this.prevSlide(), this.autorunTime
    //                 );
    //             }
    //             else {
    //                 clearInterval(this.idAutorun);
    //             }
    //         },

    //         stopAutorun() {
    //             clearInterval(this.idAutorun);
    //         }
    //     },

    //     mounted() {
    //         this.runSlider();
    //     },
    // },
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
                    <div v-for="testimonial in DataTestimonials" :key="testimonial.name"
                        class="testimonial_card d-flex flex-column text-center py-5">
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
                    </div>
                    <div class="testimonial_icons">
                        <a href=""></a>
                        <a href=""></a>
                        <a href=""></a>
                        <a href=""></a>
                        <a href=""></a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.testimonials {
    background-image: url(../assets/img/testimonial-background.jpg);
    background-size: contain cover;
    margin-top: -5rem;
}

.container {
    max-width: 1000px;
    margin: auto;
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



.img_container {
    width: 120px;
    margin: auto;

    img {
        width: 100%;
    }
}
</style>