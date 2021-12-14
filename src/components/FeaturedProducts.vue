<template>
    <section>
        <Title 
        :title="titleText"
        :subtitle="subtitleText"/>
        
    </section>
</template>

<script>
import Title from '../components/Title.vue'
export default {
  name: 'FeaturedProducts',
  components: {
      Title,
  },
  props: {
    
  },
  data () {
      return {
        titleText:"Featured Products",
        subtitleText: "Must have products from our top sellers"
      }
  }
}
</script>


<style scoped lang="scss">
    header {
        height: 70vh;
    } 
</style>