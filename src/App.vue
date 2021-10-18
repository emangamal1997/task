<template>
  <div id="app">
    <AppHeader />

    <router-view />
    <AppFooter />
  </div>
</template>
<script>
import AppHeader from "@/components/global/navbar.vue";
import AppFooter from "@/components/global/footer.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter
  }
};
</script>

<style></style>
