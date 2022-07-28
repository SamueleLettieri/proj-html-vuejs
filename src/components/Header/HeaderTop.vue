<template>
  <section id="header" class="p-2 ms_background-green">
    <div class="container d-flex justify-content-between">
      <div class="ms_font"><a class="ms_color-white" href=""><i class="fa-solid fa-phone-flip"></i> Call us a free Quote: 1.800.555.6789</a></div>
      <IconProject/>
    </div>
  </section>
</template>

<script>
import IconProject from '../IconProject.vue';

export default {
    components: {
    IconProject
}
}
</script>

<style lang="scss" scoped>
.ms_background-green{
  background-color: #69bf14;
}

.ms_font{
  font-size: 13px;
}

a{
  text-decoration: none;
}

.ms_color-white{
  color: white;
}
</style>