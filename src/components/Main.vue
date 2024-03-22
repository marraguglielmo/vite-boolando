<script>
import ProductCard from './partials/ProductCard.vue';
    export default{
        components:{
            ProductCard
        }
    }
</script>

<template>
    <div class="container d-flex">
        <ProductCard />
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
