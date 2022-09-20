<template>
  <div>
    <input
      type="text"
      placeholder="Enter your username"
      v-model="signup.username"
    />
    <br /><br />
    <input
      type="password"
      placeholder="Enter your password"
      v-model="signup.password"
    />
    <p>Choose Hobbies</p>
    <input
      type="checkbox"
      id="cricket"
      value="cricket"
      v-model="signup.hobbies"
    />
    <label for="cricket">Cricket</label>
    <input
      type="checkbox"
      id="football"
      value="football"
      v-model="signup.hobbies"
    />
    <label for="football">Football</label>

    <br />
    <p>Select Gender</p>

    <input type="radio" id="male" value="male" v-model="signup.gender" />
    <label for="male">Male</label>
    <input type="radio" id="female" value="female" v-model="signup.gender" />
    <label for="female">female</label>
    <br />
    <br />

    <button v-on:click="singUpUser">SignUp</button>
  </div>
</template>

<script>
export default {
  name: "SignUp",
  data() {
    return {
      signup: { username: null, password: null, hobbies: [], gender: null },
    };
  },

  methods: {
    singUpUser() {
      console.log(this.signup);
    },
  },
};
</script>

<style></style>
