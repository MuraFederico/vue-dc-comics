<template>
    <main>
        <section id="main-content">
            <h1>inserire contenuto</h1>
        </section>
        <nav class="nav-main">
            <ul>
                <li v-for="(navEle, index) in navList" :key="index"><a href=""><img :src="navEle.icon" :alt="navEle.name">{{ navEle.name }}</a></li>
            </ul>
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
                    icon: '../assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    icon: 'buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    icon: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    icon: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'DC POWER VISA',
                    icon: 'buy-dc-power-vis.svg'
                },
            ]
        }
    }
}
</script>

<style>

</style>