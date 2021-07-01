<template>
  <div id="nav">
    <v-app-bar id="navbar" color="blue " fixed app dense>
      <h1>Roofing and Guttering</h1>
      <v-spacer />
      <div id="deets-container">
        <a class="deet" href="mailto:bbuilding@gmail.com">
          bbuilding@gmail.com
        </a>
        <a class="deet" href="tel:+353873794038">
          +353 87 379 4038
        </a>
      </div>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style scoped>
#navbar {
  color: rgb(235, 37, 37) !important;
  background: rgb(41, 9, 158) !important;
}
.deet {
  color: rgb(202, 21, 21);
  padding: 10px;
  font-size: 1.1rem;
}
.deet:hover {
  color: rgb(235, 37, 37);
}
</style>
