<template>
  <div id="m-container">
    <div id="anchor"></div>
    <h1>Where To Find Us</h1>
    <div id="maps-container">
      <div class="map">
        <h3>
          Robinhood Industrial Estate, Clondalkin, Dublin 22
          <br />
          <a class="number-container" href="tel:+353873794038">
            <v-icon class="icon">
              mdi-phone
            </v-icon>
            <p class="number">087 379 4038</p>
          </a>
        </h3>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2383.3803655409806!2d-6.3478172841626055!3d53.3185425799733!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x48670c980fdfc0f3%3A0xcf8f97d342529e58!2sUnit%2045%2C%20Robinhood%20Industrial%20Estate%2C%20Unit%2047%2C%20Robinhood%20Rd%2C%20Robinhood%2C%20Dublin%2022!5e0!3m2!1sen!2sie!4v1625515923355!5m2!1sen!2sie"
          style="border:0;"
          loading="lazy"
        ></iframe>
      </div>
      <div class="map">
        <h3>
          Donore Business Park, Drogheda, County Louth
          <br />
          <a class="number-container" href="tel:+353870630470">
            <v-icon class="icon">
              mdi-phone
            </v-icon>
            <p class="number">087 063 0470</p>
          </a>
        </h3>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m16!1m12!1m3!1d2361.687398086872!2d-6.3656367841479575!3d53.706015830055954!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!2m1!1sDonore%20Business%20Park%2C%20Drogheda%2C%20County%20Louth!5e0!3m2!1sen!2sie!4v1625516128628!5m2!1sen!2sie"
          style="border:0;"
          loading="lazy"
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "maps",
};
</script>

<style scoped>
#m-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 50px;
  background: rgba(11, 19, 43, 0.836);
  color: aliceblue;
}
h1 {
  max-width: 75%;
  text-align: center;
}
#maps-container {
  width: 100%;
  display: flex;
  justify-content: center;
}
.map {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: 45%;
  min-width: 250px;
  max-width: 450px;
  height: 50vw;
  min-height: 350px;
  max-height: 550px;
  margin: 10px;
  padding: 10px;
}
.icon {
  font-size: 1.5rem !important;
  color: inherit !important;
}
.number {
  margin: 5px !important;
}

iframe {
  width: 100%;
  height: 100%;
}
.number-container {
  color: rgb(202, 21, 21);
  padding: 10px;
  text-decoration: none;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
}
.number-container:hover {
  color: rgb(235, 37, 37);
}

@media (max-width: 750px) {
  #maps-container {
    flex-direction: column;
    align-items: center;
  }
  .map {
    min-width: none;
    width: 90%;
    height: 50vh;
    height: 400px;
  }
}
</style>
