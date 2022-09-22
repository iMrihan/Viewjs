<template>
  <div>
    <h1>Ref in Vue Js</h1>
    <input type="text" ref="input" />
    <button v-on:click="getData">Click Me</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    getData() {
      this.$refs.input.focus();
      let val = this.$refs.input.value;
      this.$refs.input.style.color = "red";
      console.log(val);
    },
  },
};
</script>

<style></style>
