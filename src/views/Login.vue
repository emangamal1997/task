<template>
  <div class="container">
    <h3>LOGIN</h3>
    <form class="" @submit.prevent="check" action="/profile">
      <div class="mb-3">
        <label for="userName" class="form-label">User Name</label>
        <input
          type="name"
          class="form-control"
          id="userName"
          v-model="userName"
          required
        />
      </div>
      <div class="mb-3">
        <label for="userPassword" class="form-label">Password</label>
        <input
          type="password"
          class="form-control"
          id="userPassword"
          v-model="password"
          required
        />
      </div>
      <p v-if="passwordError">{{ passwordError }}</p>
      <button type="submit" class="btn">
        submit
      </button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      userName: "eman",
      password: "123",
      passwordError: ""
    };
  },
  methods: {
    check() {
      if (this.userName !== "eman" && this.password !== "123") {
        this.passwordError =
          "The user name or password you wrote is wrong, please try again..";
      } else {
        this.passwordError = "";
      }
    }
  }
};
</script>

<style lang="css" scoped>
h3 {
  color: #ef7b8c;
  text-align: center;
  padding-top: 80px;
}
form {
  padding: 40px;
  margin: auto;
  width: 50%;
}

button {
  color: #ef7b8c;
  font-weight: bold;
}
</style>
