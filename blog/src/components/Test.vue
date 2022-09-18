<template>
  <div>
    <h1>Hello from the Home component</h1>
    <h2>{{ data }}</h2>
    <h3>{{ msg }}</h3>
  </div>
</template>

<script>
export default {
  name: "Test",
  props: {
    data: String,
    msg: String,
  },
};
</script>
<style></style>
