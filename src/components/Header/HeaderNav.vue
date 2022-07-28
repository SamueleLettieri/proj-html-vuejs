<template>
    <li class="fw-bold"><a :href="item.url" :class="{ms_active: item.id === 0}" v-on:click="nweClass(item.id)">{{item.items}}</a></li>
</template>

<script>
export default {
    props:["item"],
    data: function(){
        return{
            activindex: 0,
            classVisible: false
        }
    },
}
</script>

<style lang="scss" scoped>
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

.ms_active{
    color: #69bf14;
}

</style>