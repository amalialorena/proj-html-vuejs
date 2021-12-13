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
</style>
