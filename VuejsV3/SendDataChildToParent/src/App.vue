<template>
  <h1>Sent Data Child To Parent</h1>
  <h2>{{ childUser }}</h2>
  <User :getUser="getUser" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import User from "./components/User.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    User,
  },
  data() {
    return {
      childUser: "",
    };
  },

  methods: {
    getUser(name) {
      this.childUser = name;
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
