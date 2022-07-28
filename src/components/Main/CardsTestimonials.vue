<template>
    <div class="ms_box text-center d-inline-block mt-5">
        <div><img class="ms_box-img" :src="card.image" alt=""></div>
        <h4 class="mt-4 fw-bold">{{card.name}}</h4>
        <p class="mt-4">{{card.text}}</p>
    </div>
</template>

<script>
export default {
    props:["card"]
}
</script>

<style lang="scss" scoped>
.ms_box{
    width: 350px;
    margin-left: 20px;
    margin-right: 20px;

}

.ms_box-img{
    width: 120px;
    object-fit: cover;
    border-radius: 50%;
}

h4{
    color:  #1975c0;;
}
</style>