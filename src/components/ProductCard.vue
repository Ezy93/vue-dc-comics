<template>
    <div class="product-card">
        <img :src="thumbLinks" :alt="productSeries">
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
        width: calc(100% / 6);
        text-align: start;
        h4{
            padding: 1rem 0rem;
        }
    }
</style>