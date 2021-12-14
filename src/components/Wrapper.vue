<template>
  <div>
    <Nav/>
    <Header/>
    <FeaturedProducts/>
    <Collections/>
    <BestSeller/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Nav from './nav/Nav.vue'
import FeaturedProducts from '../components/FeaturedProducts.vue'
import Collections from '../components/Collections.vue'
import BestSeller from '../components/BestSeller.vue'
import Main from '../components/Main.vue'
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
export default {
  name: 'Wrapper',
  components: {
    Nav,
    FeaturedProducts,
    Collections,
    BestSeller,
    Header,
    Main,
    Footer
  }
}
</script>


<style scoped lang="scss">


</style>
