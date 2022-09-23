<template>
  <div>
    <h1>Home Component</h1>
    <p v-for="item in list" :key="item">
      {{ item.id }} --- {{ item.email }}---- {{ item.first_name }} -----{{
        item.last_name
      }}
      <img :src="item.avatar" alt="" />
    </p>
  </div>
</template>

<script>
import { assertDeclareModuleExports } from "@babel/types";
import axios from "axios";

export default {
  name: "Home",
  data() {
    return {
      list: [],
    };
  },

  async mounted() {
    let { data } = await axios.get("https://reqres.in/api/users?page=1");
    console.log(data.data);
    this.list = data.data;
  },
};
</script>

<style></style>
