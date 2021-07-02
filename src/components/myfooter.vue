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
    <p id="compname">Roofing Repairs & Guttering - 2021</p>
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
  align-items: center;
  justify-content: space-between;
  text-align: center;
  padding: 5px 10px 5px 10px;
}
#deets-container {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  font-size: 1.1rem;
  padding: 0 !important;
  width: 40%;
}
.deet {
  color: rgb(202, 21, 21);
  padding: 10px;
  text-decoration: none;
  margin: 0 0 0 50px;
}
.deet:hover {
  color: rgb(235, 37, 37);
}
#locations {
  color: rgb(202, 21, 21);
  padding: 0 !important;
  margin: 0 !important;
}
#compname {
  padding: 0 !important;
  margin: 0 50px 0 0 !important;
}
.icon {
  font-size: 1.5rem !important;
  color: inherit !important;
}
</style>
