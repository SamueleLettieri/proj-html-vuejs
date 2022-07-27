<template>
    <div class="text-center d-inline-block ms_box">
        <div class="ms_box-img text-center"><img class="w-100" :src="card.imgag" alt=""></div>
        <h4 class="mt-4 fw-bold">{{card.title}}</h4>
        <p class="mt-3">{{card.text}}</p>
        <div class="ms_box-link mt-4 mb-4"><a class="ms_link fw-bold" :href="card.href">{{card.button}}</a></div>
    </div>   
</template>

<script>
export default {
    props:["card"]
}

</script>

<style lang="scss" scoped>
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
    color:  #1975c0;;
}

</style>