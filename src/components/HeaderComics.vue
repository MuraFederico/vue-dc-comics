<template>
  <header :class="(fixed == true) ? 'nav-down' : 'nav-up'">
      <div class="container">
          <img src="assets/img/dc-logo.png" alt="DC logo">
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
    },
    props: {
        fixed: Boolean,
    }
}
</script>

<style lang="scss" scoped>
@import "../../public/assets/styles/variables";
    header{
        background-color: white;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        z-index: 9999;
        transition: transform .5s;
        &.nav-up {
            transform: translateY(-300px);
        }
        &.nav-down{
            transform: translateY(0);
        }
    }  
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;     
    }


    li {
        margin: 0 1rem;
        // padding: 3rem 0;
        display: inline-block;

        a {
            display: inline-block;

            line-height: 100px;
            color: black;
            text-decoration: none;
            border-bottom: 5px solid transparent;

            &:hover {
                color: #0282f9;
                border-bottom: 5px solid $primary_color;
            }
        }
    }
</style>
    
