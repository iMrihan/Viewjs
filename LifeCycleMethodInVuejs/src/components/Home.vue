<template>
  <div><h1>Home</h1></div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {};
  },
  beforeMount: function () {
    console.warn("beforeMount");
  },
  mounted: function () {
    console.warn("mounted");
  },
  created: function () {
    console.warn("created");
  },
  beforeCreate: function () {
    console.warn("beforeCreated");
  },
};
</script>

<style></style>
