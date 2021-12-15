<template>
    <section>
        <Title 
            :title="titleText"
            :subtitle="subtitleText"
        />
        <Carousel :small="smallCarousel"/>
    </section>
</template>

<script>
import Title from "../components/Title.vue"
import Carousel from "../components/Carousel.vue"
export default {
  name: 'BestSeller',
  components: {
      Title,
      Carousel
  },
  data () {
      return {
        titleText: "Best Seller",
        subtitleText: "Must have products from our top sellers",
        smallCarousel: true,
      }  
  }
}
</script>


<style scoped lang="scss">


</style>