<template>
  <footer>
    <div id="col-1">
      <a
        href="https://www.google.com/maps/place/Unit+45,+Robinhood+Industrial+Estate,+Unit+47,+Robinhood+Rd,+Robinhood,+Dublin+22/@53.3185426,-6.3478173,17z/data=!3m1!4b1!4m5!3m4!1s0x48670c980fdfc0f3:0xcf8f97d342529e58!8m2!3d53.3185426!4d-6.3456286?hl=en"
        class="location-container"
      >
        <v-icon class="icon">
          mdi-map-marker
        </v-icon>
        <p class="location">
          Robinhood Industrial Estate, Clondalkin, Dublin 22
        </p>
        <br />
      </a>
      <a class="number-container" href="tel:+353873794038">
        <v-icon class="icon">
          mdi-phone
        </v-icon>
        <p class="number">087 379 4038</p>
      </a>
    </div>
    <div id="col-1">
      <a
        href="https://www.google.com/maps?q=Donore+Business+Park,+Drogheda,+County+Louth&um=1&ie=UTF-8&sa=X&ved=2ahUKEwjp4LCvuMfxAhXzrnEKHb6hDS0Q_AUoAXoECAEQAw"
        class="location-container"
      >
        <v-icon class="icon">
          mdi-map-marker
        </v-icon>
        <p class="location">
          Donore Business Park, Drogheda, County Louth
        </p>
        <br />
      </a>
      <a class="number-container" href="tel:+353870630470">
        <v-icon class="icon">
          mdi-phone
        </v-icon>
        <p class="number">087 063 0470</p>
      </a>
    </div>
    <div id="col-1">
      <a class="number-container" href="mailto:roofingr7@gmail.com">
        <v-icon class="icon">
          mdi-email
        </v-icon>
        <p class="number">roofingr7@gmail.com</p>
      </a>
      <p id="compname">Roof Repairs & Guttering.ie - 2021</p>
    </div>
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
#col-1 {
  max-width: 300px;
  min-width: 200px;
}
.location-container {
  color: rgb(202, 21, 21);
  padding: 10px;
  margin: 0;
  display: flex;
  align-items: center;
  text-decoration: none;
}
.location {
  margin: 0 !important;
}
.number-container {
  color: rgb(202, 21, 21);
  padding: 10px;
  text-decoration: none;
  display: flex;
  align-items: center;
  justify-content: stretch;
  width: 100%;
}
.number-container:hover {
  color: rgb(235, 37, 37);
}
.number {
  margin: 0 !important;
  width: 100%;
}
.email-container {
  border: solid white;
  width: 100%;
}

.icon {
  font-size: 1.5rem !important;
  color: inherit !important;
}

@media (max-width: 700px) {
  footer {
    flex-wrap: wrap;
    justify-content: center;
  }

  .number-container {
    padding: 10px;
  }
}
</style>
