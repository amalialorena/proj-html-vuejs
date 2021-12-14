<template>
    <section>
        <Title 
            :title="titleText"
            :subtitle="subtitleText"
        />
        <Carousel :small="smallCarousel"/>
        <!-- <div class="carousel">
            <div class="arrow">&#8249;</div>
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
            <div class="arrow">&#8250;</div>
        </div> -->
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
section {
    // width: 70%;
    // margin: auto;
}
//      .carousel {
//         display: flex;
//         align-items: center;
//         margin-bottom: 60px;
//         .wrapper {
//             width: calc((100% / 4) - 40px);
//             img {
//                 width: 100%
//             }
//         }
//         .arrow {
//             height: 40px;
//             width: 20px;
//             text-align: center;
//             line-height: 40px;
//             background: grey;
//             color: white;
//             flex-shrink: 0;
//         }
//     }

// }
   

</style>