<template>
  <section>
    <div class="testimonial">
      <div class="img-container">
        <img src="../assets/img/man_testimonial.png" alt="testimonial" />
      </div>
      <div class="quote">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum vitae
          sit unde voluptatem aliquid commodi omnis, optio voluptatum.
          Cupiditate, consequatur! Lorem ipsum dolor, sit amet consectetur
          adipisicing elit. Vitae, doloremque.
        </p>
        <p class="author">
           <strong>Dar&Iacute;o Pineda,</strong>  Theme fusion
        </p>
        <div class="dots"> &#9679; &#9675; </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Quotes",
};
</script>


<style scoped lang="scss">
section {
    background-image: url("../assets/img/testimonials_home_1_bg.jpg");
    height: 50vh;
    display: flex;
    justify-content: center;
    
  .testimonial {
        max-width: 1100px;
        margin: auto;
        .img-container {
            text-align: center;
            height: 60px;
            margin-bottom: 20px;
            img {
                height: 100%;
            }
        }
        .quote {
            text-align: center;
            color: white;
            font-style: italic;
            font-weight: 500;
            max-width: 700px;
            .author {
                font-style: normal;
                margin: 10px 0;
            }
        }
  }
}
</style>