<script>

    export default {
        name: "AppHeader",

        data(){
            return{
                links:[
                    {
                        "text": "CHARACTERS",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "COMICS",
                        "url": "#",
                        "current": true
                    },

                    {
                        "text": "MOVIES",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "TV",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "GAMES",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "COLLECTIBLES",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "VIDEO",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "FANS",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "NEWS",
                        "url": "#",
                        "current": false
                    },

                    {
                        "text": "SHOP",
                        "url": "#",
                        "current": false
                    },
                ]
            }
        }
    }

</script>

<template>

    <header>

        <div class="container">
            <img src="../assets/images/dc-logo.png" alt="Logo DC">

            <ul>
                <li v-for="(link, index) in links">
                    <a href="#" :class="link.current ? 'active' : '' ">{{link.text}}</a>
                </li>
            </ul>
        </div>

    </header>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;


    .container{
        @include flex;

        img{
            padding: 0.5em;
        }

        ul{
            width: 60%;
            @include flex;

            li{
                :hover{
                    color: $header-nav-hover;
                }

                a{
                    display: inline-block;
                    color: $nav-a-color;
                    font-weight: $bold;
                    height: 100%;
                    padding: 3.1em 0;
                }

                .active{
                    color: $header-nav-hover;
                    border-bottom: 3px solid $header-nav-hover;
                }
            }
        }
    }

    

</style>