<template>
  <section>
    <div class="container">
        <div class="ms_box text-center">
            <MainMiniTitle miniTitle="HEADACHE FREE"/>
            <MainTitle class="ms_w-title" title="Award Winning Moving Company"/>
            <p class="mb-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. At alias obcaecati, minus eos sapiente dignissimos sed reiciendis numquam facilis unde ut ratione quidem accusantium corrupti, illo assumenda placeat laboriosam tenetur.</p>
            <BtnProject btnLink="READ OUR TESTIMONIALS"/>
        </div>
    </div>
  </section>
</template>

<script>
import BtnProject from '../BtnProject.vue';
import MainMiniTitle from './MainMiniTitle.vue';
import MainTitle from './MainTitle.vue';
export default {
    components: {
    BtnProject,
    MainMiniTitle,
    MainTitle
}
}
</script>

<style lang="scss" scoped>
section{
    padding: 100px;
    background-color: #e9e9e9; 
}

.ms_box{
    width: 720px;
    margin: 0 auto;
}

.ms_w-title{
  margin: 0 auto;
  width: 400px;
}
</style>