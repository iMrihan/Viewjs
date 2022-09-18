<template>
  <div>
    <h1>Hello from the Home component</h1>
    <!-- <h2>{{ data }}</h2>
    <h3>{{ msg }}</h3>
    <button v-on:click="hello('call hello')">Call hello Function</button> -->

    <h1 v-if="show">Conditional Rerendering in vue.js</h1>
    <h1 v-else>Conditional Rerendering in vue.js else block</h1>
    <button v-on:click="display">Toggle Element</button>
  </div>
</template>

<script>
export default {
  name: "Test",
  props: {
    data: String,
    msg: String,
  },
  data() {
    return { show: true };
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
