<template>
  <div>
    <h1>Data Binding in Vue js</h1>
    <h1 style="white-space: pre-line">{{ message }}</h1>
    <textarea type="text" v-model="message" />
  </div>
</template>

<script>
export default {
  name: "DataBinding",
  data() {
    return {
      message: "Hi",
    };
  },
};
</script>

<style></style>
