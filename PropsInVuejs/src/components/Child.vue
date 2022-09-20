<template>
  <div>
    <h1>Child Component</h1>
    <h2 v-for="user in users" :key="user.name">
      Name: {{ user.name }} && Email: {{ user.email }}
    </h2>
  </div>
</template>

<script>
export default {
  name: "Child",
  props: ["users"],
};
</script>

<style></style>
