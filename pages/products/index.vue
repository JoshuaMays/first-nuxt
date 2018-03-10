<template>
  <div>
    <h1>Products</h1>
    <nuxt-link v-for="product in products" 
      :key="product.id"
      :to="`/products/${product.id}`"
      tag="button">
      Product #{{product.id}}
    </nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1
        },
        {
          id: 2
        }
      ]
    };
  }
}
</script>