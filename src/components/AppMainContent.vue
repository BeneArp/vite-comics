<script>
    import AppMainNav from '../components/AppMainNav.vue'
    import Cards from './Cards.vue';

    export default {
        name: "AppMainContent",
        components: {
            AppMainNav,
            Cards,
        }
    }

</script>

<template>

    <section id="main">

        <div class="container">
            <Cards/>
        </div>

    </section>

    <AppMainNav/>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #main{
        background-color: $main-background;
        padding: 5em;

        .container{
            @include flex;
            flex-wrap: wrap;
            gap: 0.8em;
        }
    }

</style>