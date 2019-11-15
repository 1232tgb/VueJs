<template>
  <div id="app">
  
    <h1>Welcome to Your Vue.js App</h1>
    <Contadores></Contadores>
  
  </div>
</template>

<script>
import Contadores from './Contadores.vue'

export default {
  name: "app",
  components: {
    Contadores
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
