<template>
    <div>
        <main>
            <section class="products">
                <div class="container">
                    <Product-Card 
                    v-for="(element,index) in productsList" 
                    :key="index"
                    :thumbLinks="element.thumb"
                    :productPrice="element.price"
                    :productSeries="element.series"
                    :productType="element.type"
                    />
                </div>
            </section>
            <section class="main-navigation">
                <div class="container">
                    <ul class="shop-links">
                        <li v-for="(element,index) in shopLinks" :key="index">
                            <a :href="element.url">
                                <img :src="require(`@/assets/images/${element.img}`)" :alt="element.name">
                                <h5>{{element.name}}</h5>
                            </a>
                        </li>
                    </ul>
                        
                </div>
            </section>
        </main>
    </div>
</template>

<script>
import ProductCard from './ProductCard.vue'


export default {
components: { ProductCard },
    name: "IndexMain",
data:function(){
        return {

            shopLinks:[
                {
                    name:"digital comics",
                    img: "buy-comics-digital-comics.png",
                    url:"#",
                },
    
                {
                    name:"dc merchandise",
                    img: "buy-comics-merchandise.png",
                    url:"#",
                },
    
                {
                    name:"subscription",
                    img: "buy-comics-subscriptions.png",
                    url:"#",
                },
    
                {
                    name:"comic shop locator",
                    img: "buy-comics-shop-locator.png",
                    url:"#",
                },
    
                {
                    name:"dc power visa",
                    img: "buy-dc-power-visa.svg",
                    url:"#",
                }
            ],

            productsList: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
                ]
        } 
        
        
    },    
    
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

    main{
        
        section.products{
            
            color: white;
            background-color: black;
            padding-bottom: 6rem;
            div.container{
                display: flex;
                flex-wrap: wrap;
            }
            
        }

        section.main-navigation{
            background-color: $brandColor;
            height: 10.5vh;
            div.container{
                height: 100%;
                ul.shop-links{
                    display: flex;
                    list-style: none;
                    justify-content: space-between;
                    height: 100%;
                    li{
                        padding: 1rem 0rem;
                        height: 100%;
                        a{
                            height: 100%;
                            text-decoration: none;
                            display: flex;
                            align-items: center;
                            text-transform: uppercase;
                            color: white;
                            img{
                                height: 100%;
                                margin: 0rem 1rem;
                            }
                        }
                    }
                }
            }
            
        }
    }
</style>