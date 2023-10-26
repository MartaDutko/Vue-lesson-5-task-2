<template>
  <product-card-list :card-list-data="raspberryList"/>
</template>

<script>
import ProductCardList from './components/ProductCardList.vue';
import { raspberryList } from "./constants/2_data_raspberry";

export default {

  name: 'App',
  components: { ProductCardList },
  data() {
    return {
      raspberryList
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
