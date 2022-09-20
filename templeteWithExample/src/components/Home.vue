<template>
  <div>
    <p v-html="rowHtml"></p>
    <h2 v-once>{{ name }}</h2>
    <h2>{{ name }}</h2>
    <h2>{{ ok ? "Yes" : "No" }}</h2>
    <button v-on:click="updateText">Click Me</button>
    <button v-bind:disabled="disableBtn" v-on:click="update">Click Me</button>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {
      name: "Rihan",
      a: 10,
      b: 15,
      ok: false,
      rowHtml: "<h1>Template in vue js</h1>",
      disableBtn: true,
    };
  },
  methods: {
    updateText() {
      this.name = "Khan";
    },
    update() {
      this.ok = !this.ok;
    },
  },
};
</script>

<style></style>
