<template>
  <main>
    <MainTop/>
    <MainServiceSolution/>
    <MainTrasporto/>
    <MainTestimonials/>
  </main>
</template>

<script>
import MainTop from './MainTop.vue';
import MainServiceSolution from './MainServiceSolution.vue';
import MainTrasporto from './MainTrasporto.vue';
import MainTestimonials from './MainTestimonials.vue';
export default {
    components: {
    MainTop,
    MainServiceSolution,
    MainTrasporto,
    MainTestimonials
}
}
</script>

<style>

</style>