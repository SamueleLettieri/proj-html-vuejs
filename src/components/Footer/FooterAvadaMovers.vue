<template>
  <li class="mb-4"><a :href="linkAvada.url" :class="{ms_active: linkAvada.id === 0}"  @click.prevent=""><span class="me-2">❯</span> {{linkAvada.text}}</a></li>
</template>

<script>
export default {
props:["linkAvada"]
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

.ms_active{
    color: $Lima;
}
</style>