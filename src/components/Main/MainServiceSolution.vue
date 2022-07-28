<template>
  <section>
    <div class="container text-center">
        <h6 class="fw-bold ms_titolino">WE ARE A PROFESSIONAL</h6>
        <h1 class="fw-bold ms_title mb-5">Full-Service Solution</h1>
        <div>
            <CardsServiceSolution v-for="(card, index) in serviceSolutionCards" :key="index"  :card="card"/>
        </div>    
    </div>
  </section>
</template>

<script>
import CardsServiceSolution from './CardsServiceSolution.vue';
export default {
    components: {
        CardsServiceSolution
    },

    data: function(){
        return{
            serviceSolutionCards:[
                {
                    img: require("../../assets/img/avada-movers-serviceonephoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
                    button: "READ MORE",
                },
                {
                    img: require("../../assets/img/avada-movers-servicetwophoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
                    button: "READ MORE",
                },
                {
                    img: require("../../assets/img/avada-movers-servicethreephoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
                    button: "READ MORE",
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
section{
    padding: 100px;
}

</style>