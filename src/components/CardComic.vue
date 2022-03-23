<template>
  <div class="card">
      <img :src="thumb" :alt="series">
      <h3>{{ series }}</h3>
  </div>
</template>

<script>
export default {
    name: 'CardComic',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<style lang="scss" scoped>
    .card {
        flex-basis: calc(100% / 6 - 1rem);
        margin: 1.5rem 0;
        display: flex;
        flex-direction: column;
        img {
            margin-bottom: 1rem;
        }
        &:hover {
            cursor: pointer;
        }
        &:hover img {
            opacity: .3;
        }
    }
</style>>

