<script>

    export default {
        name: "AppHeader",
    }

</script>

<template>

    <header>

        <div class="container">
            <img src="../assets/images/dc-logo.png" alt="Logo DC">

            <ul>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
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
                    border-bottom: 3px solid $header-nav-hover;
                }

            a{
                display: inline-block;
                color: $nav-a-color;
                font-weight: $bold;
                height: 100%;
                padding: 3.1em 0;
            }
            }
        }
    }


</style>