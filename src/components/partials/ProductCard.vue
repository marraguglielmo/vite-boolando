<script>
    export default{}
</script>

<template>
        <div class="card">
            <div class="card-img">
                <img src="../../assets/img/1.webp" alt="card1"> 
                <img class="product-hover" src="../../assets/img/1b.webp" alt="1hover">
                <!-- heart -->
                <div class="favorite">
                    <i class="fa-solid fa-heart"></i>
                </div>
                <!-- discount -->
                <div class="discount">-50%</div>
                <!-- sostenibility -->
                <div class="sostenibility">sostenibilità</div>
            </div>
            <div class="card-text">
                <h3>Levi's</h3>
                <h2>RELAXED FIT TEE UNISEX</h2>
                <span class="new-price">14.99 €</span>
                <span class="old-price">29.99 €</span>
            </div>
        </div>
</template>

<style lang="scss">
@use '../../assets/scss/partials/general';
@use '../../assets/scss/partials/utils' as *;
@use '../../assets/scss/partials/variables' as *;


    .card{
        width: calc(100% / 3);
        padding: 15px 10px;
        .card-img{
            position: relative;
            z-index: 1;
        }
        .card-text{
            line-height: 22px;
        }
        .new-price{
            color: $bg-red;
            font-weight: 600;
        }
        .old-price{
            text-decoration:line-through;
        }
        .discount{
            background-color: $bg-red;
            position: absolute;
            bottom: 40px;
            color: white;
            padding: 1px 7px;
            font-size: .8rem;
            z-index: 2;
        }
        .sostenibility{
            background-color: $bg-sostenibility;
            position: absolute;
            bottom: 40px;
            left: 50px;
            padding: 1px 7px;
            font-size: .8rem;
            color: white;
            z-index: 2;
        }
        .product-hover{
            position: absolute;
            display: none;
            top: 0;
            left: 0;
            z-index: 0;
        }
        &:hover .product-hover{
            display: block;
        }
    }
    .card#card6 .sostenibility{
        position: absolute;
        bottom: 40px;
        left: 0;
    }
    .favorite{
        background-color: white;
        position: absolute;
        top: 10px;
        right: 0;
        padding: 5px 12px;
        font-size: 1.5em;
        z-index: 2;
        i{
            &:hover{
                color: $bg-red;
                cursor: pointer;
            }
        }
    }


</style>
