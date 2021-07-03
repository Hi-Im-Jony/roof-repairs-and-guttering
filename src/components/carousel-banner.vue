<template>
  <v-carousel
    id="carousel"
    cycle
    interval="4500"
    hide-delimiters
    show-arrows-on-hover
  >
    <v-carousel-item>
      <roof-banner />
    </v-carousel-item>
    <v-carousel-item>
      <gutter-banner />
    </v-carousel-item>
    <v-carousel-item>
      <flatroof-banner />
    </v-carousel-item>
    <v-carousel-item>
      <chimney-banner />
    </v-carousel-item>
  </v-carousel>
</template>

<script>
import ChimneyBanner from "./chimney-banner.vue";
import FlatroofBanner from "./flatroof-banner.vue";
import GutterBanner from "./gutter-banner.vue";
import PhoneBtn from "./phone-btn.vue";
import RoofBanner from "./roof-banner.vue";

export default {
  name: "carouselBanner",
  components: {
    PhoneBtn,
    RoofBanner,
    GutterBanner,
    FlatroofBanner,
    ChimneyBanner,
  },
};
</script>

<style scoped>
#carousel {
  background: rgb(15, 22, 41) !important;
  height: 50vh !important;
  max-height: 498px !important;
  min-height: 350px !important;
  padding: 0 !important;
  margin: 0 !important;
}
</style>
