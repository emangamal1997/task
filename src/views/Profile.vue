<template>
  <div class="container">
    <div class="profile">
      <h1>
        Hi Eman,<br />
        we are happy to see you here again!
      </h1>
      <ul class="list-group">
        <h4>list of items you liked:</h4>
        <li class="list-group-item" v-for="item in items" :key="item.id">
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Profile",
  data() {
    return {
      items: ["Red Scarf", "Black Lazar Skirt", "White Coat", "Gray Boot"]
    };
  }
};
</script>
<style scoped>
.profile {
  padding-top: 80px;
  padding-bottom: 60px;
  text-align: center;
  margin: auto;
}
h1 {
  color: #b7defa;
  padding-bottom: 40px;
}
h4 {
  color: #ef7b8c;
  padding-bottom: 20px;
}
.list-group {
  width: 50%;
  margin: auto;
}
</style>
