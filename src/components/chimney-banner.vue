<template>
  <div id="banner-container">
    <div id="flatroof-banner"></div>
    <div id="foreground">
      <h1>CHIMNEYS</h1>
      <p>
        25 year guaranteed Chimney Installations and Chimney Repairs.
        <br />
        Call today for a free no-obligation quote!
      </p>
      <phone-btn flashing="true" />
    </div>
  </div>
</template>

<script>
import phoneBtn from "./phone-btn.vue";
export default {
  components: { phoneBtn },
  name: "flatroof-banner",
};
</script>

<style scoped>
#banner-container {
  margin: 0;
  padding: 0;
  position: relative;
}
#flatroof-banner {
  background-image: url("../assets/chimney.png");

  background-repeat: no-repeat;
  background-size: cover;
  height: 50vh;
  width: 100vw;
  padding: 0;
  margin: 0;
  color: red;
}
#foreground {
  color: rgb(236, 241, 245);
  text-shadow: 2px 2px 10px black;
  top: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  position: absolute;
  top: 0;
  font-size: 1.7rem;
  text-align: center;
  background: rgba(12, 31, 56, 0.452);
  height: 50vh;
  min-height: 350px;
}
#foreground p {
  width: 50%;
  min-width: 200px;
}
@media (min-width: 900px) {
  #flatroof-banner {
    background-attachment: fixed;
    background-position: left center;
  }
}
@media (max-width: 770px) {
  #foreground {
    font-size: 1.5rem;
  }
}
@media (max-width: 450px) {
  #foreground {
    font-size: 1.3rem;
  }
}
</style>
