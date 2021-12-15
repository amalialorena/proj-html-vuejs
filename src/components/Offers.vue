<template>
    <section>
        <div class="wrapper">
            <div class="card">
                <img src="../assets/img/promo_box_1_bg.jpg" alt=" promo box">
            </div>
            <div class="card">
                <img src="../assets/img/promo_box_2_bg.jpg" alt=" promo box">
            </div>
        </div> 
    </section>
</template>

<script>
export default {
  name: 'Offers',
  components: {
   
  }
}
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
                img {
                    width: 100%;
                }
            }
        }
    }


</style>