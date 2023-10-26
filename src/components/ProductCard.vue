<template>
    <div class="block">
        <div class="block__img">
            <img :src="cardData.imgSrc" class="img">
        </div>
        <div class="block__tittle">
            <div class="block__info">
                <img :src="cardData.logo" >
                <span class="logoName">{{cardData.companyTitle}}</span>
            </div>
            <div class="block__description"> {{cardData.description}}</div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'ProductCard',
        props: {
            cardData: {
                type: Object,
                default: ()=>({})
            },
        },
    }
</script>

<style lang="css" scoped>
.block{
    padding: 10px;
    color: white;
}
.img{
    height: 100px; 
    max-width: 100%;
    border-radius: 5px;
}
.block__info{
    display: flex;
}
.block__description{
    text-align: left;
}
</style>