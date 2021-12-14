<template>
    <section>
        <Title 
        :title="titleText"
        :subtitle="subtitleText"
        />
        <div class="categories">
            <div class="category selected">Men</div>
            <div class="category middle">Women</div>
            <div class="category">Accessories</div>
        </div>
        <div class="cards">
            <div class="card">
                <img src="../assets/img/black_elegant_leather_jacket-400x520.jpg" alt="black leather jacket">
                <h5>Black Leather Jacket</h5>
                <small>Men, Jackets, Jeans</small>
                <p><s>&dollar;235</s>&dollar;200</p>
            </div>
             <div class="card">
                <img src="../assets/img/black_leather_suit-400x520.jpg" alt="black leather jacket">
                <h5>Black Leather Suit</h5>
                <small>Men, Jackets</small>
                <p>&dollar;170</p>
            </div>
             <div class="card">
                <img src="../assets/img/blue_jacket_and_white_stripe_tee-400x520.jpg" alt="black leather jacket">
                <h5>Blue Jacket & stripe Tee</h5>
                <small>Men, Jackets, Suits</small>
                <p>&dollar;580</p>
            </div>
             <div class="card">
                <img src="../assets/img/modern_black_leather_suit-400x520.jpg" alt="black leather jacket">
                <h5> Modern Black Leather Suit</h5>
                <small>Men, Jackets</small>
                <p>&dollar;296</p>
            </div>
        </div>
        
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
section {

    .categories {
        display: flex;
        justify-content: center;
        .category {
            padding: 10px 30px;
            border: 1px solid #c0bdbd;;
            font-size: .8em;
            font-weight: 600;
            background-color: #f4f4f4;   
        }
        .middle {
            border-right: 0;
            border-left: 0;
        }
        .selected {
            background-color: white;
        }
    }
    .cards {
        display: flex;
        width: 70%;
        margin: auto;
        .card {
            margin-top: 30px;
            margin-bottom: 130px;
            width: calc(100% / 4);
            img {
                width: 100%;
            }
            small {
            font-size: .7em;
            }
            p {
                color:#3467cc;
                font-size: .8em;
                font-weight: 600;
                s {
                    font-size: .7em;
                    margin: 3px;
                }
            }
        }
     
    }


}
   

</style>