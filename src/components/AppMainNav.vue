<script>
    export default {
        name: "AppMainNav",

        data(){
            return{
                shopLinks:[
                    {
                        "text": "DIGITAL COMICS",
                        "url": "#",
                        "image": "../assets/images/buy-comics-digital-comics.png"
                    },

                    {
                        "text": "DC MERCH",
                        "url": "#",
                        "image": "../assets/images/buy-comics-merchandise.png"
                    },

                    {
                        "text": "SUBSCRIPTION",
                        "url": "#",
                        "image": "../assets/images/buy-comics-subscriptions.png"
                    },

                    {
                        "text": "COMICS SCHOP LOCATOR",
                        "url": "#",
                        "image": "../assets/images/buy-comics-shop-locator.png"
                    },

                    {
                        "text": "DC POWER VISA",
                        "url": "#",
                        "image": "../assets/images/buy-dc-power-visa.svg"
                    },
                ]
            }
        }
    }

</script>

<template>

    <section id="main-nav">

        <div class="container">
            
            <div v-for="shop in shopLinks">
                <a :href="shop.url">
                    <img src="../assets/images/buy-comics-digital-comics.png" :alt="shop.text">
                    <span>{{shop.text}}</span>
                </a>
            </div>

        </div>

    </section>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #main-nav{
        background-color: $main-nav-background;
        padding: 3em;

        .container{
            @include flex;
            justify-content: center;
            gap: 2em;

            div{
                // border: 2px solid black;
                width: calc(100% / 5);
                text-align: center;

                img{
                    vertical-align: middle;
                    margin-right: 1em;
                    height: 60px;
                    max-width: 20%;
                }

                span{
                    color: white;
                }
            }

        }
    }

</style>