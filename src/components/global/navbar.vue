<template lang="html">
  <div class="container">
    <div class="header">
      <nav class="nav justify-content-center ">
        <router-link to="/" exact class="nav-link">Home</router-link>

        <router-link to="/login" class="nav-link">Login</router-link>

        <router-link to="/profile" class="nav-link">Profile</router-link>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style lang="css" scoped></style>
