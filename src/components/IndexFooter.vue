<template>
    <div>
        <div class="top-footer">
            <div class="container">
                <div class="nav-footer">
                    <div class="ul-container">
                        <ul>
                            <li>
                                <a href="#"></a>
                            </li>
                        </ul>
                        <ul>

                        </ul>
                    </div>
                </div>
                <div class="logo-dc">
                    
                </div>
            </div>
        </div>
        <div class="bot-footer">
            <div class="container">

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexFooter',
    data: function(){
        return {
            topFooterLink:[
                {
                    title: "dc comics",
                    linkList:[
                        "Character",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    title: "shop",
                    linkList:[
                        "Shop DC",
                        "Shop DC Collectibles",
                        
                    ]
                },
                {
                    title: "dc",
                    linkList:[
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
                        
                    ]
                },
                {
                    title: "sites",
                    linkList:[
                        "DC",
                        "Mad magazine",
                        "DC kids",
                        "DC universe",
                        "DC Power Visa",
                    ]
                },
                
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
            height: 300px;
            div.logo-dc{
                height: 100%;
                background-image: url("../assets/images/dc-logo-bg.png")
            }
            
        };
        div.ul-container{
            display: flex;
            flex-direction: column;
        }
        ul{
            list-style-type: none;
            a{
                color: #576a79;
                text-decoration: none;
            }
        }
    }
</style>