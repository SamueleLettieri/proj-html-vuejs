<template>
 <h1 class="ms_title mb-4 fw-bold">{{title}}</h1>
</template>

<script>
export default {
props: ["title"]
}
</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

.ms_title{
    color: $Lima;
}

</style>