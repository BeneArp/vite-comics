<script>
    export default {
        name: "Cards",

        props:{
            menuItems: Array,
        },
    }

</script>

<template>

    <div class="card" v-for="(comic, index) in menuItems" :key="index" @mouseenter="comic.hover = true" @mouseleave="comic.hover = false">

        <div class="cover">
            <img :src="comic.thumb" alt="">
        </div>

        <span>{{comic.series}}</span>

        <div class="info" v-if="comic.hover === true ? 'hidden' : '' ">

            <span>
                Genere:
                <h5>{{ comic.type }}</h5>
            </span>
            <span>
                Prezzo:
                <h5>{{ comic.price }}</h5>
            </span>

        </div>

    </div>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .card{
        margin: 2em 0;
        width: 15%;
        cursor: pointer;
        position: relative;
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

        .info{
            width: 7vw;
            height: 7vw;
            background-color: $main-background;
            border: 2px solid $main-nav-background;
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translate(-50%);
            opacity: 0.8;
            padding: 1em 0;
            font-size: 18px;
            text-align: center;
        }

        .hidden{
            display: none;
        }
    }

</style>