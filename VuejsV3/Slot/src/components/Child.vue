<template>
  <div class="cart">
    <header>
      <slot name="header"></slot>
    </header>

    <content>
      <slot name="main"></slot>
    </content>
    <footer>
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Child",
};
</script>

<style>
.cart {
  border: 1px solid;
  width: 300px;
  height: 200px;
  margin: auto;
  margin-top: 20px;
}
</style>
