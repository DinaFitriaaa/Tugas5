<script setup>
import Navbar from './Navbar.vue'
import Carousel from './Carousel.vue'
import ProductCard from './ProductCard.vue'
import Footer from './Footer.vue'

const products = [
  { id: 1, name: 'Baju', price: 'Rp.50.000-100.00', image: '/gambar1.jpg' },
  { id: 2, name: 'Celana pria', price: 'Rp.100.00-200.00', image: '/gambar2.jpg' },
  { id: 3, name: 'Pantofel', price: 'Rp.200.00-500.00', image: '/gambar3.jpg' }
];
</script>

<template>
  <div>
    <Navbar /> 
    <Carousel />
    <div class="product-list">
      <ProductCard v-for="product in products" :key="product.id" :product="product" />
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.product-list {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  margin: 2em 0;
}
</style>
