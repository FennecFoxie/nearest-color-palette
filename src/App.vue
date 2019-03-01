<template>
  <div id="app">
    <ColorFinder />
    <Palette v-bind:colors="colors" />
  </div>
</template>

<script>
import ColorFinder from './components/ColorFinder.vue'
import Palette from './components/Palette.vue'

export default {
  name: 'app',
  components: {
    ColorFinder,
    Palette
  },
  data() {
    return {
        colors: [{
        id: 1,
        name: "$c-portland-orange",
        code: "#ff5722"
      },
      {
        id: 2,
        name: "$c-cornflower-blue",
        code: "#0054A8"
      },
      {
        id: 3,
        name: "$c-limeade",
        code: "#3dbb01"
      }]
    }
  },

}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
