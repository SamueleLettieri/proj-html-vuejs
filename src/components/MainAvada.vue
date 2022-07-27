<template>
  <main>
    <MainTop/>
    <MainServiceSolution/>
    <MainTrasporto/>
    <MainTestimonials/>
    <MainBottom/>
  </main>
</template>

<script>
import MainTop from './MainTop.vue';
import MainServiceSolution from './MainServiceSolution.vue';
import MainTrasporto from './MainTrasporto.vue';
import MainTestimonials from './MainTestimonials.vue';
import MainBottom from './MainBottom.vue';
export default {
    components: {
    MainTop,
    MainServiceSolution,
    MainTrasporto,
    MainTestimonials,
    MainBottom
}
}
</script>

<style>

</style>