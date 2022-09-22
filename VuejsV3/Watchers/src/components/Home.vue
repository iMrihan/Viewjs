<template>
  <div>
    <h1>Watchers Property in Vue Js</h1>
    <h2>{{ count }}</h2>
    <button v-on:click="count = count + 1">+</button>
    <button v-on:click="count = count - 1">-</button>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {
      count: 0,
    };
  },

  watch: {
    count(cur, prev) {
      if (cur > 5 && prev < cur) {
        // alert("stop counting")
        this.count = 0;
      }
    },
  },
};
</script>

<style></style>
