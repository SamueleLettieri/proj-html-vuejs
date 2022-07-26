<template>
  <div class="ms_jumbotron pt-4">
    <div class="container d-flex justify-content-between">
        <div><img src="../assets/img/avada-movers-logo.png" alt=""></div>
        <div>
            <ul class="d-inline-block">
                <HeaderNav v-for="(item, index) in NavItem" :key="index" :item="item"/>
            </ul>
            <div class="d-inline-block ms_link"><a href="#">FREE QUOTE</a></div>
        </div>
    </div>
  </div>
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

.ms_link{
    margin-left: 20px;
    a{
        padding: 8px 20px;
        background-color: #1975c0;
        border-radius: 20px;
        text-decoration: none;
        color: white;
        font-size: 13px;
    }
}

</style>