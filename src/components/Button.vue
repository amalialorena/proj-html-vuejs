<template>
 <button>{{data}}</button>
</template>

<script>
export default {
  name: 'Button',
  props: {
      data: String,
  }  
}
</script>


<style scoped lang="scss">
    button {
        border: 2px solid white;
        background-color: rgba(255, 255, 255, 0.1);
        color:white;
        font-weight: bold;
        padding: 10px 25px;
        border-radius: 17px;
        margin: 10px;
    }

</style>