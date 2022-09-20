<template>
  <div class="home">
    <h1>Home Component</h1>
    <Users />
    <Products />
  </div>
</template>

<script>
import Users from "./Users.vue";
import Products from "./Products.vue";

export default {
  name: "Home",
  components: {
    Users,
    Products,
  },
};
</script>

<style scoped>
.home {
  background-color: rgb(149, 127, 127);
  height: 600px;
  border: 1px solid red;
}
</style>
