<template>
    <div class="product-card">
        <div class="image-product">
            <img :src="thumbLinks" :alt="productSeries">
        </div>
        <h4>{{productSeries}}</h4>
    </div>
</template>

<script>
export default {
    name: "ProductCard",
    props:['thumbLinks','productPrice','productSeries','productType']
}
</script>

<style lang="scss" scoped>
    div.product-card{
        width: calc(100% / 6 - 1rem);
        height: 27vh;
        text-align: start;
        margin-top: 2rem;
        margin-left: .5rem;
        margin-right: .5rem;

        div.image-product{
            height: 90%;
            width: 100%;
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }

        h4{
            
            padding: 1rem 0rem;
        }
    }
</style>