<template>
  <div @wheel="toggleFixed" id="app">
    <HeaderComics
    :fixed="headerComics.fixed"
    />
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
  },
  data() {
    return {
      headerComics: {
        fixed: false
      }
    }
  },
  methods: {
    toggleFixed(event) {
      event.deltaY < 0 ? this.headerComics.fixed = true : this.headerComics.fixed = false;
      // console.log(this.headerComics.fixed)
    }
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
