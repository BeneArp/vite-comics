<script>

    export default {
        name: "AppFooter",
    }

</script>

<template>

    <footer>
        <div id="nav-container">
            <div class="container">

                <nav>

                    <div>

                        <h3>DC COMICS</h3>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                        </ul>

                        <h3>SHOP</h3>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                        </ul>

                    </div>

                    <div>

                        <h3>DC</h3>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                            <li>
                                <a href="#">Shop Collectibles</a>
                            </li>
                        </ul>

                        </div>

                        <div>
                            <h3>SITES</h3>
                            <ul>
                                <li>
                                    <a href="#">Shop DC</a>
                                </li>
                                <li>
                                    <a href="#">Shop Collectibles</a>
                                </li>
                                <li>
                                    <a href="#">Shop Collectibles</a>
                                </li>
                                <li>
                                    <a href="#">Shop Collectibles</a>
                                </li>
                                <li>
                                    <a href="#">Shop Collectibles</a>
                                </li>
                            </ul>
                        </div>
                        
                </nav>

                <img src="../assets/images/dc-logo-bg.png" alt="">

            </div>
        </div>

        <div id="footer-banner">
            <div class="container">

                <div class="button">
                    SIGN-UP NOW!
                </div>

                <div id="social">
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="../assets/images/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/images/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/images/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/images/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/images/footer-periscope.png" alt=""></a>
                </div>

            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    footer{
        // debug

        #nav-container{
            padding: 4em 0;
            background-image: url('../assets/images/footer-bg.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            position: relative;
            overflow: hidden;

            nav{
            @include flex;
            width: 30%;
            align-items: flex-start;

            h3{
                margin: 0.8em 0;
                color: $footer-title-color;
            }

            li{
                margin-bottom: 0.8em;

                a{
                    color: $footer-nav-color;
                }
            }

            }

            img{
                position: absolute;
                right: 20%;
                top: -5%;
            }
        }

        #footer-banner{
            background-color: $footer-background;
            padding: 3em 0;
            
            .container{
                @include flex;

                .button{
                    color: $footer-title-color;
                    padding: 1.3em 1em;
                    border: 2px solid rgb(2 130 249);
                    cursor: pointer;
                    font-weight: $bold;
                }

                #social{
                    width: 25%;
                    @include flex;

                    h3{
                        color: rgb(2 130 249);
                        font-weight: $bold;
                    }
                }
            }

        }
    }

</style>