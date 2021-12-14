<template>
  <div class="container">
      <div class="card">
          <img src="../assets/img/winter_collection_bg.jpg" alt="winter collection">
          <div class="description">
              <h3>
                  Winter Collection
              </h3>
              <h5>
                  STILISH AND WARM
              </h5>
              <Button 
                :text="buttonText"
                :small="style"
              />
          </div>
      </div>
      <div class="card">
          <img src="../assets/img/spring_collection_bg.jpg" alt="spring collection">
             <div class="description">
              <h3>
                  Spring Collection
              </h3>
              <h5>
                  BRIGHT AND COLORFUL
              </h5>
              <Button 
                :text="buttonText"
                :small="style"
              />
          </div>
      </div>
      <div class="card">
          <img src="../assets/img/autumn_collection_bg.jpg" alt="autumn collection">
             <div class="description">
              <h3>
                 Autumn Collection
              </h3>
              <h5>
                  RICH AND COMFORTABLE
              </h5>
              <Button 
                :text="buttonText"
                :small="style"
              />
          </div>
      </div>
  </div>
</template>

<script>
import Button from '../components/Button.vue'
export default {
  name: 'Collections',
  components: {
      Button,
  },
  data () {
    return {
        buttonText: "VIEW MORE",
        style: true,
    }
 }
}


</script>


<style scoped lang="scss">
    .container {
        display: flex;
        height: 50vh;
        .card {
            width: calc(100% / 3);
            height: 100%;
            overflow: hidden;
            position:relative;
            img {
                width: 100%;
            }
            .description {
                position: absolute;
                bottom: 50px;
                width: 100%;
                text-align: center;
                color: white;
                h3 {
                    font-size: 2em;  
                }
                h5 {
                    margin-bottom: 15px;
                    margin-top: 5px;
                }
            }
        }
    } 
    

</style>