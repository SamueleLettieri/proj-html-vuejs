<template>
  <section>
    <div class="container">
        <div class="text-end">
            <div class="ms_background-lima p-4 d-inline-block text-center">
                <h6 class="fw-bold">WE REMOVE THE HEADACHE FROM MOVING</h6>
                <h1 class="fw-bold">Move With Ease</h1>
                <hr>
                <p class="mt-4">Whith our super simple service we can take you from getting a quotes, right through to being in your new home with all of your belongings securely packed and safely delivered, even in the rooms of your choice.</p>

                <BtnProject class="mt-4" btnLink="GET A FREE QUOTE NOW"/>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import BtnProject from '../BtnProject.vue';
export default {
    components: { BtnProject }
}
</script>

<style lang="scss" scoped>
section{
    padding: 200px;
    background-image: url(../../assets/img/avada-movers-movewithease-background-new.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: top;    

}

.ms_background-lima{
    background-color: #69bf14;
    border: 15px solid #559910;
    color: white;
    width: 500px;
}
h6{
    font-size: 12px;
}

hr{
    margin-left: 50px;
    margin-right: 50px;
    width: 300px;
}

</style>