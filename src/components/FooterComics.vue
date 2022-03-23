<template>
    <footer>
        <section id="footer-main">
            <div class="container">
                <div class="container-links">
                    <ul>
                        <li class="list-title"><h3>DC COMICS</h3></li>
                        <li v-for="(link, index) in comicsList" :key="index"><a :href="link.href">{{link.name}}</a></li>
                    </ul>
                    <ul>
                        <li class="list-title"><h3>DC SHOP</h3></li>
                        <li v-for="(link, index) in shopList" :key="index"><a :href="link.href">{{link.name}}</a></li>
                    </ul>
                    <ul>
                        <li class="list-title"><h3>DC</h3></li>
                        <li v-for="(link, index) in DCList" :key="index"><a :href="link.href">{{link.name}}</a></li>
                    </ul>
                    <ul>
                        <li class="list-title"><h3>SITES</h3></li>
                        <li v-for="(link, index) in sitesList" :key="index"><a :href="link.href">{{link.name}}</a></li>
                    </ul>
                </div>
                <div class="container-logo">
                    <img src="assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>
        <div id="footer-socials">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <div class="container-socials">
                    <h2>FOLLOW US</h2>
                    <a v-for="(social, index) in socialLinks" :key="index" :href="social.href"><img :src="social.icon" alt=""></a>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterComics',
    data() {
        return {
            comicsList: [
                {
                    name: 'Characters',
                    href: '#'
                },
                {
                    name: 'Comics',
                    href: '#'
                },
                {
                    name: 'movies',
                    href: '#'
                },
                {
                    name: 'TV',
                    href: '#'
                },
                {
                    name: 'Gamses',
                    href: '#'
                },
                {
                    name: 'Videos',
                    href: '#'
                },
                {
                    name: 'News',
                    href: '#'
                },
            ],
            shopList: [
                {
                    name: 'Shop DC',
                    href: '#'
                },
                {
                    name: 'Shop DC Collectibles',
                    href: '#'
                },
            ],
            DCList: [
                {
                    name: 'Terms of Use',
                    href: '#'
                },
                {
                    name: 'Privacy Policy (New)',
                    href: '#'
                },
                {
                    name: 'Ad Choices',
                    href: '#'
                },
                {
                    name: 'Advertising',
                    href: '#'
                },
                {
                    name: 'Jobs',
                    href: '#'
                },
                {
                    name: 'Subscriptions',
                    href: '#'
                },
                {
                    name: 'CPSC Certificates',
                    href: '#'
                },
                {
                    name: 'Ratings',
                    href: '#'
                },
                {
                    name: 'Shop Help',
                    href: '#'
                },
                {
                    name: 'Contact Us',
                    href: '#'
                },
            ],
            sitesList: [
                {
                    name: 'DC',
                    href: '#'
                },
                {
                    name: 'DC UNIVERSE INFINITE',
                    href: '#'
                },
                {
                    name: 'DC Kids',
                    href: '#'
                },
                {
                    name: 'DC Shop',
                    href: '#'
                },
                {
                    name: 'DC Magazine',
                    href: '#'
                },
            ],
            socialLinks: [
                {
                    icon: 'assets/img/footer-facebook.png',
                    href: '#'
                },
                {
                    icon: 'assets/img/footer-twitter.png',
                    href: '#'
                },
                {
                    icon: 'assets/img/footer-youtube.png',
                    href: '#'
                },
                {
                    icon: 'assets/img/footer-pinterest.png',
                    href: '#'
                },
                {
                    icon: 'assets/img/footer-periscope.png',
                    href: '#'
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../../public/assets/styles/variables";

    .container {
        display: flex;
        justify-content: space-between;
        height: 100%;
    }
    #footer-main {
        height: 400px;
        overflow: hidden;
        background-image: url("../../public/assets/img/footer-bg.jpg");
        background-size: cover;
    }
    .container-links {
        padding: 2rem 0;
        display: flex;
        flex-flow: column wrap;
        color: white;
        ul {
            margin-bottom: 1rem;
            margin-right: 1.5rem;
            list-style: none;
        }
        .list-title {
            margin-bottom: .5rem;
        }
        a {
            color: gray;
            text-decoration: none;
        }
    }
    .container-logo {
        align-self: center;
    }
    #footer-socials {
        padding: 2rem;
        background-color: #303030;
        button {
            padding: .7rem;
            background-color: transparent;
            color: white;
            border: 2px solid $primary_color;
            border-radius: none;
            &:hover {
                cursor: pointer;
            }
        }
    }
    .container-socials {
        display: flex;

        h2 {
            margin: 0 .7rem;
            color: $primary_color;
        }
        a {
            margin: 0 .5rem;
        }
    }
</style>