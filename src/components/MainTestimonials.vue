<template>
  <section>
    <div class="container text-center">
        <h6 class="fw-bold">HAPPY CUSTOMERS</h6>
        <h1 class="fw-bold ms_title">Testimonials</h1>
        <div>
            <CardsTestimonials v-for="(card ,index) in testimonials" :key="index" :card="card"/>
        </div>
        <div class="ms_box-link mt-5"><a class="ms_link fw-bold" href="#">READ MORE TESTIMONIALS</a></div>
    </div>
  </section>
</template>

<script>
import CardsTestimonials from './CardsTestimonials.vue';
export default {
    components: {
        CardsTestimonials 
    },

    data: function(){
        return{
            testimonials:[
                {
                    image: require("../assets/img/avada-movers-johndoe-final.jpg"),
                    name: "John Doe",
                    text:'"Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel sapiente dolor natus architecto fugit numquam magnam aut cumque est necessitatibus."'
                },
                {
                    image: require("../assets/img/avada-movers-janedoe-final.jpg"),
                    name: "Jane Doe",
                    text:'"Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel sapiente dolor natus architecto fugit numquam magnam aut cumque est necessitatibus."'
                },
                {
                    image: require("../assets/img/avada-movers-johnsmith-final.jpg"),
                    name: "John Smith",
                    text:'"Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel sapiente dolor natus architecto fugit numquam magnam aut cumque est necessitatibus."'
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
section{
    padding: 100px;
    background-image: url(../assets/img/avada-movers-testimonial-background.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

</style>