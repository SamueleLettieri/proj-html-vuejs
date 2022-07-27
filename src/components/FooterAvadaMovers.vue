<template>
  <li class="mb-4"><a :href="linkAvada.url"><span class="me-2">❯</span> {{linkAvada.text}}</a></li>
</template>

<script>
export default {
props:["linkAvada"]
}
</script>

<style lang="scss" scoped>
li{
    
    list-style: none;

    a{
        text-decoration: none;
        color: black;
    }

    a:hover{
        color: #69bf14;
    }
}
</style>