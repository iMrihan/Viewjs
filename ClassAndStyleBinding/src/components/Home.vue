<template>
  <div>
    <h1 class="homeStyle">Class And Style Bindings</h1>
    <h1 v-bind:style="{ color: 'green' }">Style Bindings</h1>
    <h1 v-bind:style="{ color: keyColor }">Style Bindings with key</h1>
    <h1 v-bind:class="{ display: show, displayColor: show }">
      Class Bindings with objects
    </h1>
    <h1 v-bind:class="[aClass]">Class Bindings with Array</h1>
    <h1 v-bind:class="[show ? 'yesShow' : 'noShow']">
      Class Bindings with Conditioning Array
    </h1>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      show: true,
      aClass: "arrayClass",
      keyColor: "red",
    };
  },
};
</script>

<style>
.homeStyle {
  color: orange;
}

.display {
  background-color: brown;
}

.arrayClass {
  background-color: aqua;
}
</style>
