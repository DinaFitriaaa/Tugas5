<template>
  <div class="carousel">
    <div class="carousel-item">Item 1</div>
    <div class="carousel-item">Item 2</div>
    <div class="carousel-item">Item 3</div>
  </div>
</template>

<style scoped>
.carousel {
  display: flex;
  overflow: hidden;
  width: 100%;
  margin: 2em 0;
}

.carousel-item {
  min-width: 100%;
  transition: transform 0.5s ease;
}
</style>
