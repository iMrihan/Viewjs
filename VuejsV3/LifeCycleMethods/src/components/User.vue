<template>
  <h1 ref="user">User Component</h1>
</template>

<script>
export default {
  name: "User",

  beforeUnmount() {
    console.log("beforeUnmount", this.$refs["user"]);
  },
  unmounted() {
    console.log("Unmount", this.$refs["user"]);
  },
};
</script>

<style></style>
