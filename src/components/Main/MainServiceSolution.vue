<template>
  <section>
    <div class="container text-center">
        <MainMiniTitle miniTitle="WE ARE A PROFESSIONAL"/>
        <MainTitle class="mb-5" title="Full-Service Solution"/>
        <div>
            <CardsServiceSolution v-for="(card, index) in serviceSolutionCards" :key="index"  :card="card"/>
        </div>    
    </div>
  </section>
</template>

<script>
import CardsServiceSolution from './CardsServiceSolution.vue';
import MainMiniTitle from './MainMiniTitle.vue';
import MainTitle from './MainTitle.vue';
export default {
    components: {
    CardsServiceSolution,
    MainMiniTitle,
    MainTitle
},

    data: function(){
        return{
            serviceSolutionCards:[
                {
                    img: require("../../assets/img/avada-movers-serviceonephoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
                },
                {
                    img: require("../../assets/img/avada-movers-servicetwophoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
                },
                {
                    img: require("../../assets/img/avada-movers-servicethreephoto-final-400x255.jpg"),
                    title: "Two man teams",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit autem nobis quod itaque ut fugiat repellendus, cum ipsum corrupti dolor maxime.",
                    href: "#",
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