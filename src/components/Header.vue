<template>
    <header>
        <div class="title">
            <h1>
                 Brand New Arrivals
            </h1>
            <h4>
                NEW COLLECTION FROM NEW YORK
            </h4>
            <Button :text="leftButton"/>
            <Button :text="rightButton"/>
        </div>
    </header>
</template>

<script>
import Button from '../components/Button.vue'
export default {
  name: 'Header',
  components: {
      Button,
  },
  data() {
      return {
          leftButton: 'VIEW ALL',
          rightButton: 'LOOKBOOK'
      }
  }
  
}
</script>


<style scoped lang="scss">
    header {
        height: 70vh;
        background-image: url("../assets/img/home1_slide_three_bg_2.jpg");
        background-position: center;
        background-size: cover;
        display: flex;
        align-items: center;
        justify-content: center;
        .title {
            text-align: center;
            color:white;
        }
        h1 {
            font-size: 4.4em;
        }
        h4 {
            font-size: 1.6em;
            font-weight: 300;
            margin-bottom: 10px;
        }
       Button {
           margin: 0 10px;
       }
    } 
</style>