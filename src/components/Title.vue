<template>
<div class="container">
    <div class="title-with-lines">
        <hr>
        <h1>{{title}}</h1>
        <hr>
    </div>
        
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
        width: 100%;
        margin-bottom: 30px;
        .title-with-lines {
            display: flex;
            width: 100%;
            justify-content: space-around;
            align-items: center;
            margin: 60px auto 0;
            hr {
                height: 1px;
                width: 100%;
            }
             h1 {
                flex-shrink: 0;
                font-size: 2.4em;
                display: inline-block;
                padding: 0 30px;
            }
           
        }
        h4 {
            font-size: .9em;
            font-weight: 500;
            color: #585758;
            margin-bottom: 40px;
        }
       
    }

</style>