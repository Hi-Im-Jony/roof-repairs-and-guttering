<template>
  <footer>
    <div id="deets-container">
      <p id="locations">
        <v-icon class="icon">
          mdi-map-marker
        </v-icon>
        Dublin, Meath & Louth
        <br />
      </p>
      <a class="deet" href="tel:+353873794038">
        <v-icon class="icon">
          mdi-phone
        </v-icon>
        087 379 4038
      </a>
      <a class="deet" href="mailto:roofingr7@gmail.com">
        <v-icon class="icon">
          mdi-email
        </v-icon>
        roofingr7@gmail.com
      </a>
    </div>
    <p>Roofing Repairs & Guttering - 2021</p>
    <small>
      Designed by <a href="https://corneljonathan.website">CJ Web Design</a>
    </small>
  </footer>
</template>

<script>
export default {
  name: "myfooter",
};
</script>
<style scoped>
footer {
  width: 100%;
  background: rgb(10, 16, 48);
  color: aliceblue;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
#deets-container {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  width: 100%;
  font-size: 1.1rem;
  padding: 0 !important;
}
.deet {
  color: rgb(202, 21, 21);
  padding: 10px;
  text-decoration: none;
}
.deet:hover {
  color: rgb(235, 37, 37);
}
#locations {
  color: rgb(202, 21, 21);
}
.icon {
  font-size: 1.5rem !important;
  color: inherit !important;
}
</style>
