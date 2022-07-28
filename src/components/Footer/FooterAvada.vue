<template>
  <footer>
    <FooterTop/>
    <FooterBottom/>
  </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterBottom from './FooterBottom.vue';
export default {
    components: {
    FooterTop,
    FooterBottom
}
}
</script>

<style lang="scss">
footer{
  background-color: #69bf14;
  padding-top: 10px;
}
</style>