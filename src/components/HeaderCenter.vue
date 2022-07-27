<template>
  <section class="ms_jumbotron pt-4">
    <div class="container ms_box">
        <div class="d-flex justify-content-between">
            <div><img src="../assets/img/avada-movers-logo.png" alt=""></div>
            <div>
                <ul class="d-inline-block">
                    <HeaderNav v-for="(item, index) in NavItem" :key="index" :item="item"/>
                </ul>
                <div class="d-inline-block ms_box-link fw-bold"><a class="ms_link" href="#">FREE QUOTE</a></div>
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
export default {
    name: "CenterHeader",
    components: {
        HeaderNav 
    },

    data: function(){
        return{
            NavItem:[
                {
                  items: "Home",
                  url: "#",
                },

                {
                  items:"Rates",
                  url: "#",
                }, 

                {
                  items:"Testimonials",
                  url: "#",
                }, 

                {
                  items:"FAQ",
                  url: "#",
                }, 

                {
                  items:"Blog",
                  url: "#",
                },

                {
                  items:"Contact",
                  url: "#",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.ms_jumbotron{
    background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
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
    color: #93989b;
}

</style>