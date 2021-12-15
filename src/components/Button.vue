<template>
    <button :class="small? 'small':'' || blue? 'blue': ''">
        {{text}}
    </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
      text: String,
      small: Boolean,
      blue: Boolean,
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
        margin: 0 10px;
    }
    .small {
        font-size: .6em;
        padding: 8px 17px;
    }
    .blue {
        background-color: #3467c7;
        border-radius: 20px;
    }

</style>