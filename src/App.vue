<template>
  <div id="app">
     <!-- componente contenitore padre -->
    <Wrapper/>
  </div>
</template>

<script>
import Wrapper from './components/Wrapper.vue'

export default {
  name: 'App',
  components: {
    Wrapper
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
* {
  padding:0;
  margin:0;
  box-sizing: border-box;
}
body {
  font-family: 'Montserrat', sans-serif;
}
</style>
