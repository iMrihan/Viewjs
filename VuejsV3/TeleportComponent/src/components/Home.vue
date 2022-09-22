<template>
  <div>
    <h1>Home Component</h1>

    <teleport to="#footer">
      <Footer />
    </teleport>
  </div>
</template>

<script>
import Footer from "./Footer.vue";
export default {
  name: "Home",
  components: {
    Footer,
  },
};
</script>

<style></style>
