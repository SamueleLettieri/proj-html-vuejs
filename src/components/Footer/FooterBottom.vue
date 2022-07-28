<template>
  <section class="p-4">
    <div class="container text-center">
        <p><a class="ms_info" href="#"  @click.prevent=""> © Copyright 2021-2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress </a></p>
        <IconProject/>
    </div>
    <div class="text-end"><a class="ms_still" href="#header" >˄</a></div>
  </section>
</template>

<script>
import IconProject from '../Generals/IconProject.vue';
export default {
    components: { 
        IconProject 
    }
}
</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

section{
    position: relative;
}
p{
    font-size: 12px;
    color: $Bianco;
}

.ms_info{
    text-decoration: none;
    color: $Bianco;
}

.ms_still{
    padding: 3px 15px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    text-decoration: none;
    color: $Bianco;
    background-color: $Shark;
    position: absolute;
    bottom: 0px;
    right: 65px;
}
</style>