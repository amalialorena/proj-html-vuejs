<template>
  <div class="container">
      <Collection title="Winter Collection" description="STILISH AND WARM" :imageUrl="require(`../assets/img/winter_collection_bg.jpg`)" :buttonText="this.buttonText" />
      <Collection title="Spring Collection" description="BRIGHT AND COLORFUL" :imageUrl="require(`../assets/img/spring_collection_bg.jpg`)" :buttonText="this.buttonText" />
      
      <!-- TODO: MAKE DYNAMIC -->
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
      <!-- TODO: MAKE DYNAMIC -->

  </div>
</template>

<script>
import Button from '../components/Button.vue'
import Collection from './Collection.vue'
export default {
  name: 'Collections',
  components: {
      Button,
      Collection,
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

        // TODO: REMOVE THIS CSS WHEN ALL THE CARDS ARE DYNAMIC - START
        .card {
            width: calc(100% / 3);
            min-width: 500px;
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
        // TODO: REMOVE THIS CSS - END
    } 
    

</style>