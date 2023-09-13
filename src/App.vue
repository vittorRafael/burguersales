<template>
  <div class="container">
    <NavbarComp :logo="logoSrc" :alt="appName" />
    <router-view />
    <FooterComp />
  </div>
</template>
 
<script>
import FooterComp from './components/FooterComp.vue';
import NavbarComp from './components/NavbarComp.vue';
export default {
  data() {
    return {
      logoSrc: '/img/logo.png',
      appName: 'Make Your Burguer'
    }
  },
  components: {
    NavbarComp,
    FooterComp,
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  font-family: Helvetica, sans-serif;
  box-sizing: border-box;
}

.mainContainer {
  margin: 50px;
  min-height: 30rem;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}

.container {
  height: 100vh;
}
</style>
