<template>
  <h1>Slots in Vue Js</h1>
  <Child>
    <template v-slot:header> <h1>Peter</h1> </template>

    <template v-slot:main> <p>A Vue Js Product</p> </template>
    <template v-slot:footer> <button>Buy Now</button> </template>
  </Child>

  <Child>
    <template v-slot:header> <h1>Facebook</h1> </template>

    <template v-slot:main> <p>A React Js Product</p> </template>
    <template v-slot:footer> <button>Buy Now</button> </template>
  </Child>

  <!-- <Child>
    <a href="https://github.com">Go to Github</a>
  </Child>

  <Child>
    <img
      src="https://media.istockphoto.com/photos/mountain-landscape-picture-id517188688?k=20&m=517188688&s=612x612&w=0&h=i38qBm2P-6V4vZVEaMy_TaTEaoCMkYhvLCysE7yJQ5Q="
      alt=""
    />
  </Child> -->
</template>

<script>
import Child from "./Child.vue";
export default {
  name: "Home",
  components: {
    Child,
  },
};
</script>

<style></style>
