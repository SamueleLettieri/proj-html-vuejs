<template>
    <li><a :href="item.url">{{item.items}}</a></li>
</template>

<script>
export default {
    props:["item"]
}
</script>

<style lang="scss">
li{
    margin-left: 20px;
    margin-right: 20px;
    display: inline-block;
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