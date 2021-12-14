<template>
  <section>
      <Title :title="titleText" :subtitle="subtitleText"/>
      <Carousel/>
  </section>
</template>

<script>
import Title from '../components/Title.vue'
import Carousel from '../components/Carousel.vue'
export default {
  name: 'NewArrivals',
  components: {
      Title,
      Carousel,
  },
  props: {

  },
  data() {
      return {
          titleText: "New Arrivals",
          subtitleText: "Brand new products from top designers",
          
      }
  }
}
</script>


<style scoped lang="scss">
  

</style>
