<script>
import ProductCard from './partials/ProductCard.vue';
import products from '../assets/data/products'
    export default{
        data(){
            return{
                products
            }
        },
        components:{
            ProductCard
        }
    }
</script>

<template>
    <div class="container d-flex">
        <ProductCard 
            v-for="product in products.products"
            :key="product.id"
            :cardImg="product.frontImage"
            :cardImgBack="`../../assets/img/${product.backImage}`"
            :cardBrand="product.brand"
            :cardName="product.name"
            :cardPrice="product.price"
        />
        
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/partials/utils' as *;


    h1{
        font-size: 5em;
        text-align: center;
        margin-top: 3em;
    }
</style>
