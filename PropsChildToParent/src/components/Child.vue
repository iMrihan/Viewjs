<template>
  <div>
    <button v-on:click="updateTitle">Update Parent Title</button>
  </div>
</template>

<script>
export default {
  name: "Child",
  methods: {
    updateTitle() {
      this.$emit("ChangeTitle", "Parent Updated");
    },
  },
};
</script>

<style></style>
