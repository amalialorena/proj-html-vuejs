<template>
  <section>
      <Title 
      :title="titleText" 
      :subtitle="subtitleText"
      />
      <div class="cards">
          <div class="card">
              <div class="img-container">
                  <img src="../assets/img/post_img_12-320x202.jpg" alt="">
              </div>
              <h5>Nam libero tempore, cum</h5>
              <p class="date">September 19th, 2015 | 0 comments</p>
              <p>Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet</p>
          </div>
             <div class="card">
              <div class="img-container">
                  <img src="../assets/img/post_img_11-700x441.jpg" alt="">
              </div>
              <h5>Nam libero tempore, cum</h5>
              <p class="date">September 19th, 2015 | 0 comments</p>
              <p>Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet</p>
          </div>
             <div class="card">
              <div class="img-container">
                  <img src="../assets/img/post_img_10-700x441.jpg" alt="">
              </div>
              <h5>Nam libero tempore, cum</h5>
              <p class="date">September 19th, 2015 | 0 comments</p>
              <p>Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet</p>
          </div>
      </div>
  </section>
</template>

<script>
import Title from '../components/Title.vue'
export default {
  name: 'Blog',
  components: {
      Title,
  },
  data () {
      return {
          titleText:"From Our Blog",
          subtitleText: "the latest Classic Shop news"
      }
  }
}
</script>
    
<style scoped lang="scss">
section {
    padding-bottom: 60px;
    border-bottom: 1px solid grey;
     .cards {
        width: 70%;
        margin: auto;
        display: flex;
        min-width: 1100px;
        max-width: 1200px;
        .card {
            width: calc(100% / 3);
            min-width: 200px;
            margin: 10px;
            .img-container {
                width: 100%;
                img {
                    width: 100%;
                }
            }
            .date {
                font-size: .7em;
                margin-bottom: 7px;
                margin-top: 2px;
            }
            p {
                font-size: .8em;
                color: #585758;

            }
        }
    }
}
   
  

</style>