<script setup>
const props = defineProps({
  product: {
    type: Object,
    required: true
  }
});
</script>

<template>
  <div class="product-card">
    <img :src="product.image" :alt="product.name" />
    <h2>{{ product.name }}</h2>
    <p>{{ product.price }}</p>
  </div>
</template>

<style scoped>
.product-card {
  border: 1px solid #ddd;
  padding: 1em;
  margin: 1em;
  text-align: center;
  width: 200px;
}

.product-card img {
  width: 100%;
  height: auto;
}
</style>
