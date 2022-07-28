<template>
  <section>
    <div class="container text-center">
        <MainMiniTitle miniTitle="HAPPY CUSTOMERS"/>
        <MainTitle title="Testimonials"/>
        <div>
            <CardsTestimonials v-for="(card ,index) in testimonials" :key="index" :card="card"/>
        </div>
        <BtnProject class="mt-5" btnLink="READ MORE TESTIMONIALS"/>
    </div>
  </section>
</template>

<script>
import CardsTestimonials from './CardsTestimonials.vue';
import BtnProject from '../Generals/BtnProject.vue';
import MainMiniTitle from './MainMiniTitle.vue';
import MainTitle from './MainTitle.vue';
export default {
    components: {
    CardsTestimonials,
    BtnProject,
    MainMiniTitle,
    MainTitle
},

    data: function(){
        return{
            testimonials:[
                {
                    image: require("../../assets/img/avada-movers-johndoe-final.jpg"),
                    name: "John Doe",
                    text:'"Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel sapiente dolor natus architecto fugit numquam magnam aut cumque est necessitatibus."'
                },
                {
                    image: require("../../assets/img/avada-movers-janedoe-final.jpg"),
                    name: "Jane Doe",
                    text:'"Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel sapiente dolor natus architecto fugit numquam magnam aut cumque est necessitatibus."'
                },
                {
                    image: require("../../assets/img/avada-movers-johnsmith-final.jpg"),
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
    background-image: url(../../assets/img/avada-movers-testimonial-background.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

</style>