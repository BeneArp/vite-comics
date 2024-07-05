<script>

    export default {
        name: "AppFooter",
    }

</script>

<template>

    <footer>
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
    </footer>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    footer{
        padding: 4em 0;
        background-image: url('../assets/images/footer-bg.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        overflow: hidden;
        // debug

        nav{
            @include flex;
            width: 30%;
            align-items: flex-start;

            h3{
                margin: 0.8em 0;
                color: $footer-title-color;
            }

            li{
                margin-bottom: 0.4em;

                a{
                    color: $footer-nav-color;
                }
            }

        }

        img{
            position: absolute;
            right: 20%;
            top: -15%;
        }
    }

</style>