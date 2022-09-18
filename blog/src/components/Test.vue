<template>
  <div>
    <h1>Hello from the Home component</h1>
    <!-- <h2>{{ data }}</h2>
    <h3>{{ msg }}</h3>
    <button v-on:click="hello('call hello')">Call hello Function</button> -->

    <!-- <h1 v-if="show">Conditional Rerendering in vue.js</h1>
    <h1 v-else>Conditional Rerendering in vue.js else block</h1>
    <button v-on:click="display">Toggle Element</button> -->

    <table border="1px">
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
      </tr>

      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.email }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "Test",
  props: {
    data: String,
    msg: String,
  },
  // data() {
  //   return { show: true };
  // },
  data() {
    return {
      users: [
        { id: 1, name: "peter", email: "peter@gmail.com" },
        { id: 2, name: "sam", email: "sam@gmail.com" },
        { id: 3, name: "brute", email: "brute@gmail.com" },
      ],
    };
  },
  methods: {
    // hello(data) {
    //   alert(data);
    // },

    display() {
      this.show = !this.show;
    },
  },
};
</script>
<style></style>
