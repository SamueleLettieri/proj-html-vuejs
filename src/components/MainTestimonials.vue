<template>
  <section>
    <div class="container text-center">
        <h6 class="fw-bold">HAPPY CUSTOMERS</h6>
        <h1 class="fw-bold ms_title">Testimonials</h1>
        <div>
            <CardsTestimonials/>
        </div>
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
                    image: "../assets/img/avada-movers-johndoe-final.jpg",
                    name: "John Doe",
                    text:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime."
                },
                {
                    image: "../assets/img/avada-movers-janedoe-final.jpg",
                    name: "Jane Doe",
                    text:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime."
                },
                {
                    image: "../assets/img/avada-movers-johnsmith-final.jpg",
                    name: "John Smith",
                    text:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime."
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