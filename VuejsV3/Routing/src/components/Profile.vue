<template>
  <h1>{{ profile }} Profile Page</h1>
</template>

<script>
import { useRoute } from "vue-router";

export default {
  name: "Profile",
  data() {
    return {
      profile: "",
    };
  },
  created() {
    const route = useRoute();
    this.profile = route.params.name;
  },
};
</script>

<style></style>
