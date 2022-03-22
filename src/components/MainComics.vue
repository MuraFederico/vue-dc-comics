<template>
    <main>
        <section id="main-content">
            <div class="container">
                <h1>inserire contenuto</h1>
            </div>
        </section>
        <nav class="nav-main">
            <div class="container">
                <ul>
                    <li v-for="(navEle, index) in navList" :key="index">
                        <a href="">
                            <div class="container-img">
                                <img :src="navEle.icon" :alt="navEle.name">
                            </div>
                            
                            {{ navEle.name }}
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </main>
</template>

<script>
export default {
    name: 'MainComics',
    data() {
        return {
            navList: [
                {
                    name: 'DIGITAL COMICS',
                    icon: 'assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    icon: 'assets/img/buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    icon: 'assets/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    icon: 'assets/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'DC POWER VISA',
                    icon: 'assets/img/buy-dc-power-visa.svg'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #main-content {
        background-color: black;
        color: white;
    }

    .nav-main {
        padding: 3rem 0;
        text-align: center;
        background-color: #0282f9;
        
        li {
            margin: 0 1.5rem;
            display: inline-block;

            a {
                display: flex;
                justify-content: space-evenly;
                align-items: center;
                color: white;
                text-decoration: none;

                .container-img {
                    height: 50px;

                    img {
                        height: 100%;
                    }
                }
            }
        }
        
    }
</style>