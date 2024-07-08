<script>
    export default {
        name: "Cards",

        props:{
            menuItems: Array,
        }
    }

</script>

<template>

    <div class="card" v-for="(comic, index) in menuItems" :key="index">

        <div class="cover">
            <img :src="comic.thumb" alt="">
        </div>

        <span>{{comic.series}}</span>

    </div>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .card{
        margin: 2em 0;
        width: 15%;
        cursor: pointer;
        // debug

        .cover{
            background-color: lightblue;
            overflow: hidden;
            height: 9vw;
            width: 100%;

            img{
                display: block;
                width: 100%;
                object-fit: cover;
            }
        }

        span{
            display: block;
            color: white;
            margin-top: 1em;
            text-transform: uppercase;
        }
    }

</style>