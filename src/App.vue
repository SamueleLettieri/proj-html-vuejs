<template>
  <div id="app">
    <HeaderAvada/>
    <MainAvada/>
    <FooterAvada />
  </div>
</template>

<script>


import FooterAvada from './components/Footer/FooterAvada.vue'
import HeaderAvada from './components/Header/HeaderAvada.vue'
import MainAvada from './components/Main/MainAvada.vue'

export default {
  name: 'App',
  components: {
    FooterAvada,
    HeaderAvada,
    MainAvada
}
}
</script>

<style lang="scss">
  @import "~bootstrap/scss/bootstrap.scss";
  @import "./css/general.scss"
</style>
