<template>
  <section class="bg-count">
    <div class="text-center py-8 sm:text-center">
      <h5 class="text-center text-2xl font-bold tracking-tight sm:text-center sm:text-6xl">Market CAP</h5>
      <h1 class="">Lorem ipsum dolor sit amet consectetur, adipisicing elit.</h1>

      <div class="products">
        <CardComponent 
          v-for="product in products" :key="product.color" :product="product"
        />
      </div>
      
    </div>
</section>
</template>

<script>
import CardComponent from './CardComponent.vue';

export default {
    name: "CounterComponent",

    components: {
      CardComponent,
    },

    data() {
      return {
        products: [
          {
            title: 'MARKET CAP',
            color: 'gold',
            bgText: 'CNT',
            src: require('../assets/cnt-gold.png')
          },
          {
            title: 'TOTAL CNT MINTED',
            color: 'red',
            bgText: 'CNT',
            src: require('./../assets/cn-red-two.png')
          },
          {
            title: 'TOTAL CNT REDEEMED',
            color: 'silver',
            bgText: 'CNT',
            src: require('./../assets/cnt-silver.png')
          },
        ]
      }
    }
}
</script>

<style scoped>
  .bg-count{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    width: 100vw;
    min-height: 100vh;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-content: center;
  }

  .products{
    display: flex;
    max-width: 1280px;
    padding: 25px;
    margin: 0 auto;
  }


</style>