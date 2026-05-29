<template>
  <div>
    <Navbar />
    <Hero />
    <Products />
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import Hero from './components/Hero.vue';
import Navbar from './components/Navbar.vue';
import Products from './views/Products.vue';


export default {
  components: {
    Navbar,
    Hero,
    Products,
    Footer
  }
}
</script>
