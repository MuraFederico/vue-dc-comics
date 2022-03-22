<template>
  <header>
      <div class="container">
          <img src="../assets/img/dc-logo.png" alt="DC logo">
          <ul>
              <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{ link.name }}</a></li>
          </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComics',
    data() {
        return {
            links: [
                {
                    href: '#',
                    name: 'CHARACTERS'
                },
                {
                    href: '#',
                    name: 'COMICS'
                },
                {
                    href: '#',
                    name: 'MOVIES'
                },
                {
                    href: '#',
                    name: 'TV'
                },
                {
                    href: '#',
                    name: 'GAMES'
                },
                {
                    href: '#',
                    name: 'COLLECTIBLES'
                },
                {
                    href: '#',
                    name: 'VIDEOS'
                },
                {
                    href: '#',
                    name: 'FANS'
                },
                {
                    href: '#',
                    name: 'NEWS'
                },
                {
                    href: '#',
                    name: 'SHOP'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;       
    }

    li {
        display: inline-block;
    }
</style>
    
