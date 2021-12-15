<template>
  <section>
    <div class="wrapper">
      <div class="card">
        <img src="../assets/img/promo_box_1_bg.jpg" alt=" promo box" />
        <div class="description">
          <h3>70% Off</h3>
          <h5>Lorem ipsum dolor sit amet consectetur adipisicing elit. </h5>
          <Button :text="buttonText"/>
        </div>
      </div>
      <div class="card">
        <img src="../assets/img/promo_box_2_bg.jpg" alt=" promo box" />
        <div class="description">
          <h3>Free Shipping</h3>
          <h5>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum</h5>
          <Button :text="buttonText"/>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Button from "../components/Button.vue"
export default {
  name: "Offers",
  components: {
      Button,
  },
  data () {
      return {
          buttonText:"VIEW MORE",
      }
  }
};
</script>


<style scoped lang="scss">
section {
  background-image: url("../assets/img/bkgd_confetti-compressor.jpg");
  background-size: cover;
  background-position: center;
  .wrapper {
    width: 70%;
    min-width: 1100px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    padding: 70px 0;
    .card {
      width: 48%;
      position: relative;
      img {
        width: 100%;
      }
    .description {
        position: absolute;
        bottom: 50px;
        width: 100%;
        color: white;
        width: 300px;
        transform:translate(20%, -25%);
        h3 {
            font-size: 2.8em;  
        }
        h5 {
            margin-bottom: 15px;
            margin-top: 5px;
            font-size: 1em;
        }
    }
    }
  }
}
</style>