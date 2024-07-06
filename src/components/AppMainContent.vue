<script>
    import AppMainNav from '../components/AppMainNav.vue'

    export default {
        name: "AppMainContent",
        components: {
            AppMainNav,
        }
    }

</script>

<template>

    <section id="main">

        <div class="container">
            <h1>--> Content here <--</h1>
        </div>

    </section>

    <AppMainNav/>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #main{
        background-color: $main-background;
        padding: 3em;

        h1{
            font-size: 30px;
            font-weight: $bold;
            color: white;
        }
    }

</style>