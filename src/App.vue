<template>
  <v-app>
    <navbar />
    <home />
  </v-app>
</template>

<script>
import navbar from "./components/navbar.vue";
import Home from "./views/Home.vue";

export default {
  name: "App",
  components: { navbar, Home },
  data: () => ({
    //
  }),
};
</script>

<style scoped>
* {
  font-family: Helvetica, sans-serif;
}
</style>
