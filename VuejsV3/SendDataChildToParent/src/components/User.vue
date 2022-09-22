<template>
  <div>
    <h1>User Component</h1>
    <button v-on:click="getUser(userName)">Send User Name</button>
  </div>
</template>

<script>
export default {
  name: "User",
  data() {
    return {
      userName: "Rihan Khan",
    };
  },

  props: {
    getUser: Function,
  },
};
</script>

<style></style>
