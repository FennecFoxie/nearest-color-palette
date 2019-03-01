<template>
  <div id="app">
    <!-- <ColorFinder /> -->
  </div>
</template>

<script>
import ColorFinder from './components/ColorFinder.vue'

export default {
  name: 'app',
  components: {
    ColorFinder
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
