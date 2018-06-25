<template>
<div id="product" class="product">
    <img :src = "product.img" class="product_img"/>
    <h2 class="product_title">{{ title }}</h2>
    <h3 class="product_price">${{ product.price }}</h3>
    <p class="product_description"> {{ product.description }}</p>
</div>
</template>
<script>
export default {
    name: 'product',
    props: {
        title: String,
        product: Object 
    }
}
</script>
<style scoped>
.product {
    text-align:left;
    border:1px solid red;
    padding:1em;
    margin:2em 1em;
}
.product:after {
    content:"";
    display:block;
    clear:both;
}
.product_title {
    color: #666;
    font-size:200%;
    margin-bottom:0;
}
.product_price {
    margin-top:0;
}
.product_img {
    float:right;
    max-width:100%;
    height:auto;
}
</style>