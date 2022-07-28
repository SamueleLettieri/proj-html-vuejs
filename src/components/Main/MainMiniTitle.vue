<template>
  <h6 class="fw-bold ms_titolino">{{miniTitle}}</h6>
</template>

<script>
export default {
props: ["miniTitle"]
}
</script>

<style lang="scss" scoped>
@import "../../css/variables.scss";

.ms_titolino{
    color: $SilverChalice;
}
</style>