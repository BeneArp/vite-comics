<script>
    export default {
        name: "AppMainNav",
    }

</script>

<template>

    <section id="main-nav">

        <div class="container">
            
            <div>
                <a href="#">
                    <img src="../assets/images/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </a>
            </div>

            <div>
                <a href="#">
                    <img src="../assets/images/buy-comics-merchandise.png" alt="">
                    <span>DC MERCH</span>
                </a>
            </div>

            <div>
                <a href="#">
                    <img src="../assets/images/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </a>
            </div>

            <div>
                <a href="#">
                    <img src="../assets/images/buy-comics-shop-locator.png" alt="">
                    <span>COMICS SCHOP LOCATOR</span>
                </a>
            </div>

            <div>
                <a href="#">
                    <img src="../assets/images/buy-dc-power-visa.svg" alt="">
                    <span>DC POWER VISA</span>
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