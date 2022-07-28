<template>
  <header>
    <HeaderTop/>
    <HeaderCenter/>
    <HeaderBottom/>
  </header>
</template>

<script>
import HeaderTop from './HeaderTop.vue';
import HeaderCenter from './HeaderCenter.vue';
import HeaderBottom from './HeaderBottom.vue';

export default {
components: {
    HeaderTop,
    HeaderCenter,
    HeaderBottom
}
}
</script>

<style>

</style>