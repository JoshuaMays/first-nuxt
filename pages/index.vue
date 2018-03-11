<template>
  <section class="container">
    <h1>Welcome Home</h1>
    <div>
      <button class="button--green" @click="$router.push('/products')">Go to Products</button>
    </div>
    
  </section>
</template>

<script>

export default {
  layout: 'default'
}
</script>

