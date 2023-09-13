<template>
  <div>
    <BannerComp />
    <div class="mainContainer">
      <h1>Monte o seu Burguer: </h1>
      <BurguerForm />
    </div>
  </div>
</template>

<script>
import BannerComp from '@/components/BannerComp.vue';
import BurguerForm from '@/components/BurguerForm.vue';
export default {
  components: { BannerComp, BurguerForm },
  name: "HomeView",
};
</script>
