<template>
    <main>
        <section id="main-content">
            <div class="container">
                <h1>inserire contenuto</h1>
            </div>
        </section>
        <MainNav/>
    </main>
</template>

<script>
import MainNav from "./MainNav.vue";

export default {
    name: 'MainComics',
    components: {
        MainNav
    }
}
</script>

<style lang="scss" scoped>
    #main-content {
        background-color: black;
        color: white;
    }
</style>