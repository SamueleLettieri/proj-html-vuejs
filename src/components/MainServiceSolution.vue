<template>
  <section>
    <div class="container text-center">
        <h6 class="fw-bold ms_titolino">WE ARE A PROFESSIONAL</h6>
        <h1 class="fw-bold ms_title mb-5">Full-Service Solution</h1>
        <div>
            <CardsServiceSolution/>
        </div>    
    </div>
  </section>
</template>

<script>
import CardsServiceSolution from './CardsServiceSolution.vue';
export default {
    components: {
        CardsServiceSolution
    }
}
</script>

<style lang="scss" scoped>
section{
    padding: 100px;
}

</style>