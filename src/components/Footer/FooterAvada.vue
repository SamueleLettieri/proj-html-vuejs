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
@import "../../css/variables.scss";

footer{
  background-color: $Lima;
  padding-top: 10px;
}
</style>