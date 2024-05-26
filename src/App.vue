<template>
  <div>
    <Header />
    <ProductCategories />
    <FeaturedProducts />
    <PurchaseSteps />
    <foter />.
   
  </div>
</template>

<script>
import Header from './layouts/Header.vue'
import HeroSection from './components/HeroSection.vue'
import ProductCategories from './components/kategoriproduk.vue'
import FeaturedProducts from './components/produkunggulan.vue'
import PurchaseSteps from './components/Carapembelian.vue'
import cara from './layouts/carousel.vue'
import foter from './components/Footer.vue'


export default {
  components: {
    Header,
    HeroSection,
    ProductCategories,
    FeaturedProducts,
    PurchaseSteps,
    foter,
    cara,
  
  }
}
</script>