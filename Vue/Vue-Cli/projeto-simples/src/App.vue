<!--<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
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
</style>-->


<template>
  <div id="app">
    <MyVue msg="#"></MyVue>
    <MyOtherVue></MyOtherVue>

    <HelloWorld msg="Olá Mundo"></HelloWorld>
  </div>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import MyVue from "./components/MyVue.vue";
import MyOtherVue from "./components/MyOtherVue.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
    MyVue,
    MyOtherVue
  },
  data: function() {
    return {
      dados: "teste"
    };
  }
};
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