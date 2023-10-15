<template>
  <div class="product">
    <div class="'product-inner ' + product.color">
        <div class="product-text-wrap">
            <h2 class="bg-text">{{ product.bgtext }}</h2>
        </div>
        <div class="product-image-wrap">
            <img :src="product.src" class="image" alt="" />
        </div>
        <div class="product-detail">
            <h2>{{ product.title }}</h2>
            <p>Lorem, ipsum dolor.</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "CardComponent",

    props: ['product']
}
</script>

<style scoped>
    .product{
        flex: 1 1 33.333%;
        width: 100%;
        padding: 25px;
    }

    .product-inner {
        position: relative;
        padding: 25px;
        box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
    }

    .product-inner.gold{
        background-image: linear-gradient(to bottom right, #24D484, #116432);
    }

    .product-inner.red{
        background-image: linear-gradient(to bottom right, #24D484, #116432);
    }

    .product-image-wrap .image {
        width: 100%;
    }

</style>