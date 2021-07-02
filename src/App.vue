<template>
  <v-app>
    <navbar />
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import navbar from "./components/navbar.vue";

export default {
  name: "App",
  components: { navbar },
  data: () => ({
    //
  }),
};
</script>

<style scoped>
* {
  padding: 0 !important;
  margin: 0 !important;
}
</style>
