<template>
    <div class="d-inline-block ms_box-link fw-bold"><a class="ms_link" href="#"  @click.prevent="">{{btnLink}}</a></div>
</template>

<script>
export default {
props: ["btnLink"]
}
</script>

<style lang="scss" scoped>
@import "../css/variables.scss";

.ms_box-link{
    margin-left: 20px;
    .ms_link{
        padding: 8px 20px;
        background-color: $Denim;
        border-radius: 20px;
        text-decoration: none;
        color: $Bianco;
        font-size: 13px;
    }
}
</style>