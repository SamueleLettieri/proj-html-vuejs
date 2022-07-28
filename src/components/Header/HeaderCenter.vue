<template>
  <section class="ms_jumbotron pt-4">
    <div class="container ms_box">
        <div class="d-flex justify-content-between">
            <LogoMovers/>
            <div>
                <ul class="d-inline-block">
                    <HeaderNav v-for="item in NavItem" :key="item.id" :item="item"/>
                </ul>
                <BtnProject btnLink="FREE QUOTE"/>
            </div>
        </div>
        <div class="d-flex flex-column justify-content-center align-items-center ms_box">
            <h6 class="fw-bold">MOVING WITHOUT THE HASSLE</h6>
            <h1 class="fw-bold">WE MAKE IT SIMPLE</h1>
            <h6 class="fw-bold">PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</h6>
        </div>
    </div>    

  </section>
</template>

<script>
import HeaderNav from './HeaderNav.vue';
import LogoMovers from '../Generals/LogoMovers.vue';
import BtnProject from '../Generals/BtnProject.vue';


export default {
    name: "CenterHeader",
    components: {
    HeaderNav,
    LogoMovers,
    BtnProject
},

    data: function(){
        return{
            NavItem:[
                {
                  items: "Home",
                  url: "#",
                  id: 0,
                },

                {
                  items:"Rates",
                  url: "#",
                  id: 1,
                }, 

                {
                  items:"Testimonials",
                  url: "#",
                  id: 2,
                }, 

                {
                  items:"FAQ",
                  url: "#",
                  id: 3,
                }, 

                {
                  items:"Blog",
                  url: "#",
                  id: 4,
                },

                {
                  items:"Contact",
                  url: "#",
                  id: 6,
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

.ms_jumbotron{
    background-image: url(../../assets/img/avada-movers-homeherobackground-final.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 600px;
}


.ms_box{
    height:90%;
}

h1{
    font-size: 50px;
}

h6{
    font-size: 12px;
    color: $OsloGray;
}

.ms_active{
    color: $Lima;
}

</style>