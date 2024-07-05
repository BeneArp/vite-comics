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

    header{
        // debug
    }

    .container{
        @include flex;
        padding: 0.5em;

        ul{
            width: 60%;
            @include flex;

            li{
                :hover{
                    color: $header-nav-hover;
                    border-bottom: 3px solid $header-nav-hover;
                }

            a{
                color: $nav-a-color;
                font-weight: $bold;
                padding: 2.5em 0.5em;
            }
            }
        }
    }


</style>