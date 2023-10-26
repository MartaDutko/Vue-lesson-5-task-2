<template>
    <div class="wrapper">
        <product-card v-for="card in cardListData" :key="card.id" :card-data="card"/>
    </div>
</template>

<script>
import ProductCard from './ProductCard.vue'
    export default {
components: { ProductCard },
        name:'ProductCardList',
        props: {
            cardListData: {
                type: Array,
                default: ()=>[]
            },
        },
    }
</script>

<style lang="css" scoped>
.wrapper{
    display: flex;
    justify-content: center;
    background-color: rgb(32, 31, 31);
}
</style>