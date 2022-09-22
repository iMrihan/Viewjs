<template>
  <div>
    <h1>Computed Property</h1>
    <h2>{{ dollors * rupeesVal - discount }}</h2>
    <h2>{{ getResult }}</h2>
    <h2>{{ getResultMethod() }}</h2>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      dollors: 100,
      rupeesVal: 70,
      discount: 10,
    };
  },

  methods: {
    getResultMethod() {
      return this.dollors * this.rupeesVal - this.discount;
    },
  },

  // we use computed property for complicated calculation
  computed: {
    getResult() {
      return this.dollors * this.rupeesVal - this.discount;
    },
  },
};
</script>

<style></style>
