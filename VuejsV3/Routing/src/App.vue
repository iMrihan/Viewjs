<template>
  <router-link to="/">Home</router-link><br />
  <router-link to="/login">Login</router-link> <br />
  <router-link to="/profile/anil">Anil Profile Page</router-link>
  <br />
  <router-link to="/profile/peter">Peter's Profile Page</router-link>
  <br />
  <router-link to="/profile/bruce">Bruce Profile Page</router-link>
  <br />

  <router-view></router-view>
</template>

<script>
export default {
  name: "App",
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
