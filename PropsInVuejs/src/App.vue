<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1>Props in Vue js</h1>
  <!-- <Child name="Rihan Khan" /> -->
  <!-- <Child v-bind:name="userName" /> -->

  <Child v-bind:users="users" />
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
      users: [
        { name: "Rihan", email: "rihan@gmail.com" },
        { name: "Praveen", email: "praveen@gmail.com" },
        { name: "Ashish", email: "ashish@gmail.com" },
        { name: "Sonu", email: "sonu@gmail.com" },
      ],
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
