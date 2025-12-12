<script setup>
import ProductCard from './components/ProductCard.vue'
import Header from './components/Header.vue'
import Navbar from './components/navbar.vue'
</script>

<template>
  <main class="appContainer">
    <Header />
    <Navbar />
    <div class="productsContainer">
      <ProductCard
        name="Wooden Sofa Chair"
        price="800.000"
        category="Chair"
        ratings="4.9"
        image-url="/images/furniture_1.jpg"
      />
      <ProductCard
        name="Wooden Sofa Chair"
        price="800.000"
        category="Chair"
        ratings="4.9"
        image-url="/images/furniture_1.jpg"
      />
      <ProductCard
        name="Wooden Sofa Chair"
        price="800.000"
        category="Chair"
        ratings="4.9"
        image-url="/images/furniture_1.jpg"
      />
    </div>
  </main>
</template>

<style>
:root {
  --primary-color:
    #224a25, --accent-color: #febb2e, --foreground-color: #212121, --background-color: #ffffff;
}

@font-face {
  font-family: 'creato display';
  src: url('/font/CreatoDisplay-Regular.otf') format('truetype');
}

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
<style scoped>
.productsContainer {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  width: auto;
  margin: 25px 100px;
}
</style>
