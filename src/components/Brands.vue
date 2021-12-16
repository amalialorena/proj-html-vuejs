<template>
  <section>
    <div class="container">
      <h4>BRAND LOGOS</h4>
      <div class="logos">
        <div class="logo">
          <img src="../assets/img/b_logotype_6.png" alt="authentic" />
        </div>
        <div class="logo">
          <img src="../assets/img/b_logotype_7.png" alt="the yard" />
        </div>
        <div class="logo">
          <img src="../assets/img/b_logotype_1.png" alt="authentic" />
        </div>
        <div class="logo">
          <img src="../assets/img/b_logotype_2.png" alt="authentic" />
        </div>
        <div class="logo">
          <img src="../assets/img/b_logotype_3.png" alt="authentic" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Brands",
};
</script>
<style scoped lang="scss">
section {
  background-color: #f4f4f4;
  text-align: center;
  padding-top: 50px;
  padding-bottom: 20px;
  .container {
    width: 70%;
    max-width: 1100px;
    margin: auto;
    h4 {
        font-weight: 400;
        color: #797878;
    }
    .logos {
        display: flex;
        .logo {
            width: calc(100% / 5);
            padding: 30px;
            max-width: 300px;
            img {
                width: 100%;
            }
        }
    }
  }
}
</style>