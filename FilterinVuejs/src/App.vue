<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h2>Filter in Vue Js</h2>
  <h2>{{ name }}</h2>
  <Home />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Home from "./components/Home.vue";

export default {
  name: "App",
  components: {
    Home,
  },

  data() {
    return {
      name: "Rihan Khan",
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
