<template>
    <div class="card">
        <img :src="this.imageUrl" :alt="this.title">
        <div class="description">
            <h3>
                {{this.title}}
            </h3>
            <h5>
                {{this.description}}
            </h5>
            <Button 
            :text="this.buttonText"
            :small="true"
            />
        </div>
    </div>
</template>

<script>
import Button from '../components/Button.vue'
export default {
  name: 'Collection',
  props: {
      imageUrl: String,
      title: String,
      description: String,
      buttonText: String,
      buttonUrl: String, // TODO: use this prop to generate anchor tag for button
  },
  components: {
      Button,
  },
}


</script>


<style scoped lang="scss">
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
</style>