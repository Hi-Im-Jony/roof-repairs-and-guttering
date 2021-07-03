<template>
  <v-carousel cycle interval="4500" hide-delimiters show-arrows-on-hover>
    <v-carousel-item>
      <roof-banner />
    </v-carousel-item>
    <v-carousel-item>
      <gutter-banner />
    </v-carousel-item>
  </v-carousel>
</template>

<script>
import GutterBanner from "./gutter-banner.vue";
import PhoneBtn from "./phone-btn.vue";
import RoofBanner from "./roof-banner.vue";

export default {
  name: "carouselBanner",
  components: {
    PhoneBtn,
    RoofBanner,
    GutterBanner,
  },
};
</script>

<style scoped>
.item {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
  color: rgb(236, 241, 245);
  text-shadow: 2px 2px 10px black;
  font-size: 1.7rem;
  text-align: center;
}
.item p {
  width: 50%;
  min-width: 200px;
}

@media (max-width: 770px) {
  .item {
    font-size: 1.5rem;
  }
}
@media (max-width: 450px) {
  .item {
    font-size: 1.3rem;
  }
}
</style>
