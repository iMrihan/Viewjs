<template>
  <div>
    <h1>Home Component</h1>
    <!-- <input type="text" v-model.lazy="data" /> -->
    <input type="number" v-model.number="data" />

    <h2>Data is : {{ data }}</h2>

    <h2>Data is : {{ typeof data }}</h2>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      data: "",
    };
  },
};
</script>

<style></style>
