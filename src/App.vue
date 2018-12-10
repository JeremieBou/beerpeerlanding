<template>
  <div id="app">
    <BasePage />
  </div>
</template>

<script>
import BasePage from './components/BasePage.vue'

export default {
  name: 'app',
  components: {
    BasePage
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
}
</style>
