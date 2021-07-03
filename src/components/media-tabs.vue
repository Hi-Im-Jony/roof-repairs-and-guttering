<template>
  <div id="container">
    <h1>
      Gallery
    </h1>
    <v-tabs fixed-tabs background-color="#DC143C" color="white" dark>
      <v-tab>
        Roofing
      </v-tab>
      <v-tab>
        Guttering
      </v-tab>
      <v-tab>
        Chimneys
      </v-tab>
      <v-tab-item>
        <div class="tab-content">
          <roofing-imgs />
        </div>
      </v-tab-item>
      <v-tab-item>
        <div class="tab-content">
          <guttering-imgs />
        </div>
      </v-tab-item>
      <v-tab-item>
        <div class="tab-content">
          <chimney-imgs />
        </div>
      </v-tab-item>
    </v-tabs>
  </div>
</template>

<script>
import roofingImgs from "./roofing-imgs.vue";
import gutteringImgs from "./guttering-imgs.vue";
import ChimneyImgs from "./chimney-imgs.vue";

export default {
  components: {
    roofingImgs,
    gutteringImgs,
    ChimneyImgs,
  },
  name: "mediaTabs",
};
</script>

<style scoped>
#container {
  padding: 30px 20vw 50px 20vw;
  background: rgba(11, 19, 43, 0.836);
  width: 100%;
  text-align: center;
  color: aliceblue;
  margin: 50px 0 0 0;
}
.tab-content {
  height: 50vh;
  color: black;
  overflow-y: scroll;
}

@media (max-width: 660px) {
  #container {
    padding: 20px 10vw 20px 10vw;
  }
}
</style>
