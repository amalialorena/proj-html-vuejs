<template>
  <div>
    <Nav/>
    <Header/>
    <FeaturedProducts/>
    <Collections/>
    <BestSeller/>
    <Offers/>
    <NewArrivals/>
    <Quotes/>
    <Blog/>
    <Shop/>
    <Brands/>
    <Footer/>
  </div>
</template>

<script>
import Nav from './nav/Nav.vue'
import Header from '../components/Header.vue'
import FeaturedProducts from '../components/FeaturedProducts.vue'
import Collections from '../components/Collections.vue'
import BestSeller from '../components/BestSeller.vue'
import Offers from '../components/Offers.vue'
import NewArrivals from '../components/NewArrivals.vue'
import Quotes from '../components/Quotes.vue'
import Blog from '../components/Blog.vue'
import Shop from '../components/Shop.vue'
import Brands from '../components/Brands.vue'
import Footer from '../components/Footer.vue'
export default {
  name: 'Wrapper',
  components: {
    Nav,
    Header,
    FeaturedProducts,
    Collections,
    BestSeller,
    Offers,
    NewArrivals,
    Quotes,
    Blog,
    Shop,
    Brands,
    Footer
  }
}
</script>


<style scoped lang="scss">
  

</style>
