<script>

    export default {
        name: "AppFooter",

        data(){
            return{
                comicsLinks:[
                    {
                        "text": "Charaters",
                        "url": "#",
                    },

                    {
                        "text": "Comics",
                        "url": "#",
                    },

                    {
                        "text": "Movies",
                        "url": "#",
                    },

                    {
                        "text": "TV",
                        "url": "#",
                    },

                    {
                        "text": "Games",
                        "url": "#",
                    },

                    {
                        "text": "Videos",
                        "url": "#",
                    },

                    {
                        "text": "News",
                        "url": "#",
                    },

                ],

                shopLinks:[
                    {
                        "text": "Shop DC",
                        "url": "#",
                    },

                    {
                        "text": "Shop DC Collectibles",
                        "url": "#",
                    },
                ],

                DcLinks:[
                    {
                        "text": "Terms Of Use",
                        "url": "#",
                    },

                    {
                        "text": "Privacy Policy (new)",
                        "url": "#",
                    },

                    {
                        "text": "Ad Choices",
                        "url": "#",
                    },

                    {
                        "text": "Advertising",
                        "url": "#",
                    },

                    {
                        "text": "Jobs",
                        "url": "#",
                    },

                    {
                        "text": "Subscriptions",
                        "url": "#",
                    },

                    {
                        "text": "Talent Workshops",
                        "url": "#",
                    },

                    {
                        "text": "CPSC Certificates",
                        "url": "#",
                    },

                    {
                        "text": "Ratingss",
                        "url": "#",
                    },

                    {
                        "text": "Shop Help",
                        "url": "#",
                    },

                    {
                        "text": "Contact Us",
                        "url": "#",
                    },
                ],

                SiteLinks:[
                    {
                        "text": "DC",
                        "url": "#",
                    },

                    {
                        "text": "MAD Magazine",
                        "url": "#",
                    },

                    {
                        "text": "DC Kids",
                        "url": "#",
                    },

                    {
                        "text": "DC Universe",
                        "url": "#",
                    },

                    {
                        "text": "DC Power Visa",
                        "url": "#",
                    },
                ],

                socialLinks:[
                    {
                        "url": "#",
                        "image": "../assets/images/footer-facebook.png",
                        "alt": "Facebook Logo"
                    },

                    {
                        "url": "#",
                        "image": "../assets/images/footer-twitter.png",
                        "alt": "Twitter Logo"
                    },

                    {
                        "url": "#",
                        "image": "../assets/images/footer-youtube.png",
                        "alt": "YouTube Logo"
                    },

                    {
                        "url": "#",
                        "image": "../assets/images/footer-pinterest.png",
                        "alt": "Pinterest Logo"
                    },

                    {
                        "url": "#",
                        "image": "../assets/images/footer-periscope.png",
                        "alt": "Periscope Logo"
                    },
                ]
            }
        }
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
                            <li v-for="link in comicsLinks">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>

                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="link in shopLinks">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>

                    </div>

                    <div>

                        <h3>DC</h3>
                        <ul>
                            <li v-for="link in DcLinks">
                                <a :href="link.url">{{link.text}}</a>
                            </li>
                        </ul>

                        </div>

                        <div>
                            <h3>SITES</h3>
                            <ul>
                                <li v-for="link in SiteLinks">
                                    <a :href="link.url">{{link.text}}</a>
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
                    <a :href="social.url" v-for="social in socialLinks"><img src="../assets/images/footer-facebook.png" :alt="social.alt"></a>
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
            gap: 2em;

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
                top: -2%;
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