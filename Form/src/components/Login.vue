<template>
  <div>
    <p v-if="error.length">
      <b>Please Correct the Following Error</b>
      <ul>
        <li v-for="e in error" v-bind:key="e.id">
          {{e}}
        </li>
      </ul>
    </p>
    <form @submit="login">
      <input type="text" placeholder="Enter your name" v-model="name" />
      <br />
      <br />
      <input
        type="password"
        placeholder="Enter your password"
        v-model="password"
        autocomplete="on"
      />
      <br />
      <br />
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      error: [],
      name: null,
      password: null,
    };
  },

  methods: {
    login(e) {

      console.log("hello");
      e.preventDefault();
      this.error = [];
      if (this.name && this.password) {
        console.log("No Error");
      }
      if (!this.name) {
        this.error.push("username is required");
      }
      if (!this.password) {
        this.error.push("password is required");
      }
     
    },
  },
};
</script>

<style></style>
