<template>
  <div id="app">
    <HeaderComics></HeaderComics>
    <MainComics/>
    <FooterComics/>
  </div>
</template>

<script>
import HeaderComics from './components/HeaderComics.vue'
import MainComics from "./components/MainComics.vue";
import FooterComics from "./components/FooterComics.vue";

export default {
  name: 'App',
  components: {
    HeaderComics,
    MainComics,
    FooterComics
  }
}
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  .container {
    width: 80%;
    margin: 0 auto;
  }
</style>
