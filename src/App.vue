<script setup>
import ProductCard from './components/ProductCard.vue'
import Header from './components/Header.vue'
import Navbar from './components/navbar.vue'
</script>

<template>
  <main class="appContainer">
    <Header />
    <Navbar />
    <div>
      <ProductCard />
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
<style scoped></style>
