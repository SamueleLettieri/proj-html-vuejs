<template>
  <li class="mb-4"><a :href="linkPost.url" @click.prevent=""><span class="me-2">❯</span> {{linkPost.text}}</a></li>
</template>

<script>
export default {
    props:["linkPost"]
}
</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

li{
    
    list-style: none;

    a{
        text-decoration: none;
        color: black;
    }

    a:hover{
        color: $Lima;
    }
}
</style>