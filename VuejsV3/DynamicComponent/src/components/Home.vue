<template>
  <div>
    <h1>Dynamic Component</h1>
    <button @click="tab = 'Java'">Java</button>
    <button @click="tab = 'Php'">Php</button>
    <button @click="tab = 'Node'">Node</button>

    <component :is="tab" />
  </div>
</template>

<script>
import Java from "./Java.vue";
import Php from "./Php.vue";
import Node from "./Node.vue";

export default {
  name: "Home",
  components: {
    Java,
    Php,
    Node,
  },

  data() {
    return {
      tab: "Java",
    };
  },
};
</script>

<style></style>
