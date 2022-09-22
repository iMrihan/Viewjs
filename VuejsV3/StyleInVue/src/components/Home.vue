<template>
  <div>
    <h1>Style In Vue Js with Dynamically</h1>

    <!-- <h2 :class="{ green: colorChange, err: true, other: true }">component</h2> -->
    <h2 :class="applyStyle">component</h2>

    <button v-on:click="colorChange = !colorChange">Apply Style</button>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {
      colorChange: false,
    };
  },

  computed: {
    applyStyle() {
      return {
        green: this.colorChange,
        err: true,
        other: true,
      };
    },
  },
};
</script>

<style>
.green {
  background: green;
  width: 300px;
}
.err {
  color: red;
}
.other {
  font-size: 45px;
}
</style>
