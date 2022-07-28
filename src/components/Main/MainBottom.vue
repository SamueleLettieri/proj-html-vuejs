<template>
  <section>
    <div class="container">
        <div class="text-center ms_box">
            <MainTitle title="Request A Free Quote"/>
            <p class="mt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. A ipsam asperiores ratione error autem aut, eum fugiat, accusamus veniam iste pariatur tempora rem! Dolores, minus quaerat deleniti vero quod tempore?</p>
            <BtnProject class="mt-4" btnLink="CLICK HERE"/>
        </div>
    </div>
  </section>
</template>

<script>
import BtnProject from '../Generals/BtnProject.vue';
import MainTitle from './MainTitle.vue';
export default {
    components: { 
      BtnProject, 
      MainTitle 
    }
}
</script>

<style lang="scss" scoped>
section{
    padding: 100px;
    background-image: url(../../assets/img/avada-movers-request-quote-background.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.ms_box{
    margin: 0 auto;
    width: 700px;
}

</style>