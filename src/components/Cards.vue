<script>
    export default {
        name: "Cards",

        data(){

        }
    }

</script>

<template>

    <div class="card">

        <div class="cover">
            <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        </div>

        <span>ACTION COMICS</span>

    </div>

    <div class="card">

        <div class="cover">
            <img src="https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg" alt="">
        </div>
        
        <span>ACTION COMICS</span>

    </div>

    <div class="card">

        <div class="cover">
            <img src="https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg" alt="">
        </div>
        
        <span>ACTION COMICS</span>

    </div>

    <div class="card">

        <div class="cover">
            <img src="https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg" alt="">
        </div>
        
        <span>ACTION COMICS</span>

    </div>

    <div class="card">

        <div class="cover">
            <img src="https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg" alt="">
        </div>
        
        <span>ACTION COMICS</span>

    </div>

    <div class="card">

        <div class="cover">
            <img src="https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg" alt="">
        </div>
        
        <span>ACTION COMICS</span>

    </div>
    <div class="card">

<div class="cover">
    <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

<div class="card">

<div class="cover">
    <img src="https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

<div class="card">

<div class="cover">
    <img src="https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

<div class="card">

<div class="cover">
    <img src="https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

<div class="card">

<div class="cover">
    <img src="https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

<div class="card">

<div class="cover">
    <img src="https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg" alt="">
</div>

<span>ACTION COMICS</span>

</div>

</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .card{
        margin: 2em 0;
        // debug

        .cover{
            background-color: lightblue;
            overflow: hidden;
            height: 9vw;
            width: 9vw;

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
        }
    }

</style>