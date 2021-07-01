<template>
  <div id="nav">
    <v-app-bar id="navbar" flat fixed app dense>
      <a id="nav-title" href="/"><h1>Roofing and Guttering</h1></a>

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
  color: white !important;
  background: rgb(53, 55, 196) !important;
}
#nav-title {
  color: white;
  text-decoration: none;
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
