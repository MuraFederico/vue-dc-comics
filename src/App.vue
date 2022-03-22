<template>
  <div id="app">
    <HeaderComics></HeaderComics>
    <MainComics/>
  </div>
</template>

<script>
import HeaderComics from './components/HeaderComics.vue'
import MainComics from "./components/MainComics.vue";

export default {
  name: 'App',
  components: {
    HeaderComics,
    MainComics
  }
}
</script>

<style lang="scss">
  .container {
    width: 1200px;
    margin: 0 auto;
  }
</style>
