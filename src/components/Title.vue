<template>
<div class="container">
    <h1>{{title}}</h1>
    <h4>{{subtitle}}</h4>
</div>
 
</template>

<script>
export default {
  name: 'Button',
  props: {
      title: String,
      subtitle: String,
  }  
}
</script>

<style scoped lang="scss">
    .container {
        text-align: center;
        h1 {
            margin-top: 80px;
            margin-bottom: 8px;
            font-size: 2.4em;
            position: relative;
            display: inline-block;
        }
        h1::after, h1::before{
            content: '';
            width: 70%;
            position: absolute;
            border-bottom: 1px solid #c0bdbd;
            top: 50%;
            margin: 0 20px
        }
        h1::before {
            left:-268px;
        }
        h4 {
            font-size: .9em;
            font-weight: 500;
            color: #585758;
            margin-bottom: 40px;
        }
    }

</style>