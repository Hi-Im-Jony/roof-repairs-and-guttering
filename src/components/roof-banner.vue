<template>
  <div id="banner-container">
    <div id="roof-banner"></div>
    <div id="foreground">
      <h1>ROOFING</h1>
      <p>
        25 year guaranteed Roofing Installations and Roofing repairs.
        <br />
        Call today for a free no-obligation quote!
      </p>
      <phone-btn />
    </div>
  </div>
</template>

<script>
import phoneBtn from "./phone-btn.vue";
export default {
  components: { phoneBtn },
  name: "roof-banner",
};
</script>

<style scoped>
#banner-container {
  margin: 0;
  padding: 0;
  position: relative;
}
#roof-banner {
  background-image: url("../assets/roof.jpg");
  background-attachment: fixed;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  filter: grayscale(20%);
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
}
#foreground p {
  width: 50%;
  min-width: 740px;
}
</style>
