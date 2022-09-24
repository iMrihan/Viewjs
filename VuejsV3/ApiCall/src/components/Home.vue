<template>
  <div>
    <h1>User Data</h1>

    <ul class="item" v-for="item in list" :key="item">
      <li>{{ item.id }}</li>
      <li>{{ item.email }}</li>
      <li>{{ item.first_name }}</li>
      <li>{{ item.last_name }}</li>
      <li>
        <img :src="item.avatar" alt="" />
      </li>
    </ul>
  </div>
</template>

<script>
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

<style>
.item {
  display: flex;
}
.item li {
  border: 1px solid;
  display: inline-block;
  padding: 20px;
  text-align: center;
}
</style>
