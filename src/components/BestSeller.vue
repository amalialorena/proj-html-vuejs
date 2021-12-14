<template>
    <section>
        <Title 
            :title="titleText"
            :subtitle="subtitleText"
        />
        <div class="carousel">
            <div class="wrapper">
                <img src="../assets/img/spring_printed_dress-200x260.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/modern_love_tee-200-260.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/black_leather_jacket-200x260.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/black_elegant_leather_jacket-200x260.jpg" alt="">
            </div>
             <div class="wrapper">
                <img src="../assets/img/hipster_black_top-200x260.jpg" alt="">
            </div>
        </div>
    </section>
</template>

<script>
import Title from "../components/Title.vue"
export default {
  name: 'BestSeller',
  components: {
      Title,
  },
  data () {
      return {
        titleText: "Best Seller",
        subtitleText: "Must have products from our top sellers",
      }  
  }
}
</script>


<style scoped lang="scss">
section {
    width: 70%;
    margin: auto;
     .carousel {
        display: flex;
    }

}
   

</style>