<template lang="html">
  <div class="topnav">
    <div class="container">
      <router-link to="/" class="nav-link">Home</router-link>

      <router-link to="/login" class="nav-link">Login</router-link>

      <router-link to="/profile" class="nav-link">Profile</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style lang="css" scoped>
/* The navbar container */
.topnav {
  overflow: hidden;
  background-color: #ef7b8c;
}

/* Navbar links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Links - change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}
</style>
