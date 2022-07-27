<template>
  <section class="p-5">
    <div class="container d-flex">
        <div class="ms_box mx-5">
            <h6 class="fw-bold">ABOUT</h6>
            <p class="mt-4 mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt adipisci repellat, maxime excepturi quod modi laboriosam voluptate suscipit doloribus.</p>
            <LogoMovers/>
        </div>    
        <div class="d-flex justify-content-between ms_width ms-5">
            <div>
                <h6 class="fw-bold mb-4">AVADA MOVERS</h6>
                <ul>
                    <FooterAvadaMovers v-for="(linkAvada, index) in linksAvadaMovers" :key="index" :linkAvada="linkAvada"/>
                </ul>
            </div>
             <div>
                <h6 class="fw-bold mb-4">RECENT POSTS</h6>
                <ul>
                    <FooterRecentPosts v-for="(linkPost, index) in linksRecentPosts" :key="index" :linkPost="linkPost"/>
                </ul>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import LogoMovers from './LogoMovers.vue';
import FooterAvadaMovers from './FooterAvadaMovers.vue';
import FooterRecentPosts from './FooterRecentPosts.vue';
export default {
    components: {
    LogoMovers,
    FooterAvadaMovers,
    FooterRecentPosts,
},

    data: function(){
        return{
            linksAvadaMovers: [
                {
                    text:"Home",
                    url:"#",
                },
                {
                    text:"Rates",
                    url:"#",
                },
                {
                    text:"Testimonials",
                    url:"#",
                },
                {
                    text:"Blog",
                    url:"#",
                },
                {
                    text:"Free Quote",
                    url:"#",
                },
            ],

            linksRecentPosts: [
                {
                    text:"Heading Out To College?",
                    url:"#",
                },
                {
                    text:"Moving Your Business?",
                    url:"#",
                },
                {
                    text:"Outstanding Quality",
                    url:"#",
                },
                {
                    text:"Cost of Moving",
                    url:"#",
                },
                {
                    text:"Best Moving Tips",
                    url:"#",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section{
    background-color: white;
}
.ms_box{
    width: 300px;
}

.ms_width{
    width: 700px;
}

ul{
    padding: 0;
}
</style>