<template>
    <div class="text-center d-inline-block ms_box">
        <div class="ms_box-img text-center"><img class="w-100" :src="card.img" alt=""></div>
        <h4 class="mt-4 fw-bold">{{card.title}}</h4>
        <p class="mt-3">{{card.text}}</p>
        <BtnProject class="pb-4" btnLink="READ MORE"/>
    </div>   
</template>

<script>
import BtnProject from '../Generals/BtnProject.vue';
export default {
    props: ["card"],
    components: {
         BtnProject 
        }
}

</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

.ms_box{
    width: 330px;
    margin-left: 20px;
    margin-right: 20px;
    border: 15px solid #f5f5f5;
}

.ms_box-img{
    width: 300px;
    border-bottom: 15px solid #f5f5f5;
}

h4{
    color: $Denim;
}

</style>