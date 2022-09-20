<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1>Send Props Child to Parent</h1>
  <h2>{{ title }}</h2>
  <Child v-on:changeTitle="updateTitle($event)" />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Child from "./components/Child.vue";

export default {
  name: "App",
  components: {
    Child,
  },
  data() {
    return {
      title: "Props Tutorial",
    };
  },
  methods: {
    updateTitle(title) {
      this.title = title;
    },
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
