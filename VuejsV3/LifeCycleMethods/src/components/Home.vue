<template>
  <div>
    <h1>Home Component</h1>
    <button v-on:click="show = !show">Toggle Component</button>
    <User v-if="show" />
  </div>
</template>

<script>
import User from "./User.vue";
export default {
  name: "Home",
  data() {
    return {
      show: true,
    };
  },
  components: {
    User,
  },
};
</script>

<style></style>
