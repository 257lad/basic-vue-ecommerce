<template>
  <div>
    <Navbar />
    <Hero /> <!-- v-if -->

    <!-- router -->
    <ProductsPage />

    <Footer /> <!-- v-if -->
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import Hero from './components/Hero.vue';
import Navbar from './components/Navbar.vue';
import ProductsPage from './views/ProductsPage.vue';


export default {
  components: {
    Navbar,
    Hero,
    ProductsPage,
    Footer
  }
}
</script>
