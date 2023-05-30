<script>
export default {
    props: {
        DataInstructors: Array,
    },

};
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="info_instructors d-flex align-items-center">
                        <div>
                            <h2>Your Instructors</h2>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto ipsam laborum cupiditate
                                accusantium
                                mollitia odit quasi distinctio nemo impedit ullam vitae.</p>
                        </div>
                        <div>
                            <button>MORE ABOUT US</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <div v-for="instructor in this.DataInstructors" :key="instructor.name" class="card_instructors">
                        <img :src="instructor.img" :alt="instructor.img">
                        <h5>{{ instructor.name }}</h5>
                        <div>
                            <span><i class="fa-brands fa-facebook"></i></span>
                            <span><i class="fa-brands fa-twitter"></i></span>
                            <span><i class="fa-brands fa-instagram"></i></span>
                        </div>
                        <p>{{ instructor.text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.container {
    max-width: 1000px;
}
</style>