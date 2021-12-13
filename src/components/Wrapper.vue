<template>
  <div>
    <Nav/>
    <Header/>
    <Main/>
    <Footer/>
    
    <!-- <img src="../assets/img/post_img_11-300x188.jpg" alt="prova">
    <img src="../assets/img/post_img_11-320x202.jpg" alt="prova"> -->
  </div>
</template>

<script>
import Nav from '../components/Nav.vue'
import Main from '../components/Main.vue'
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
export default {
  name: 'Wrapper',
  components: {
    Nav,
    Header,
    Main,
    Footer
  }
}
</script>


<style scoped lang="scss">


</style>
