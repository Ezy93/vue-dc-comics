<template>
    <div>
        <div class="top-footer">
            <div class="container">
                <div class="nav-footer">
                    <div class="ul-vertical">
                        <ul>
                            <li>
                                <h4>dc commics</h4>
                            </li>
                            <li v-for="(element,index) in dcComicsLinks" :key="index">
                                <a href="#">{{element}}</a>
                            </li>
                        </ul>
                        <ul>
                            <li>
                                <h4>shop</h4>
                            </li>
                            <li v-for="(element,index) in shopLinks" :key="index">
                                <a href="#">{{element}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="ul-horizontal">
                        <ul>
                            <li>
                                <h4>dc</h4>
                            </li>
                            <li v-for="(element,index) in dcLinks" :key="index">
                                <a href="#">{{element}}</a>
                            </li>
                        </ul>
                        <ul>
                            <li>
                                <h4>sites</h4>
                            </li>
                            <li v-for="(element,index) in sitesLinks" :key="index">
                                <a href="#">{{element}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="logo-dc">
                    
                </div>
            </div>
        </div>
        <div class="bot-footer">
            <div class="container bottom-f">
                <div>
                    <button>
                        <a href="#">sign-up now!</a>
                    </button>
                </div>
                <div class="bot-footer-links">
                    <h3>follow us</h3>
                    <ul class="footer-img-links">
                        <li v-for="(element,index) in footerLinks" :key="index">
                            <a href="#">
                                <img :src='`${element}`' alt="">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexFooter',
    data: function(){
        return {
            dcComicsLinks:[
                        "Character",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ],
            shopLinks:[
                        "Shop DC",
                        "Shop DC Collectibles",
                        
                    ],
            dcLinks:[
                        "Terms of Use",
                        "Privacy policy(New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshop",
                        "CPCS Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us"
                        
                    ],
            sitesLinks:[
                        "DC",
                        "Mad magazine",
                        "DC kids",
                        "DC universe",
                        "DC Power Visa",
                    ],
            footerLinks:[
                "../assets/images/footer-facebook.png",
                
            ]
                
                
            
        }
    },
    methods:{
        
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
    div{

        div.top-footer{
            background-image: url("../assets/images/footer-bg.jpg");
                div.container{
                    display: flex;
                    justify-content: space-between;

                    div.nav-footer{
                        width: 40%;
                        text-align: start;
                        display: flex
                    }

                    div.logo-dc{
                        background-image: url("../assets/images/dc-logo-bg.png");
                        background-position: center;
                        background-size: cover;
                        width: 45%;
                        
                    }
                }
        };

        div.bot-footer{
            background-color: #303030;
            div.bottom-f{
                display: flex;
                justify-content: space-between;
                    div.bot-footer-links{
                        display: flex;
                        align-items: center;
                        ul.footer-img-links{
                            display: flex;
                        }
                    }
            }
        }
        div.ul-vertical{
            display: flex;
            flex-direction: column;
        }
        div.ul-horizontal{
            display: flex;
        }
        ul{
            list-style-type: none;
            padding: 1rem;
            li{
                padding-bottom: .3rem;
                a{
                    color: #576a79;
                    text-decoration: none;
                    font-size: .7rem;
                }
            }
        }
        h4{
            text-transform: uppercase;
            color: white;
            margin-bottom: 1rem;
        }
        h3{
            text-transform: uppercase;
            color: $brandColor;
        }

        button{
            margin: 1.35rem 0rem ;
            padding: .9rem;
            background-color: transparent;
            border: 2px solid $brandColor;
                a{
                    text-transform: uppercase;
                    color: white;
                    text-decoration: none;
                }
        }
    }
</style>