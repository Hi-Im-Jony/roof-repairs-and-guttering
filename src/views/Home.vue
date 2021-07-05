<template>
  <div id="homepage">
    <carousel-banner />
    <paint />
    <intro-text />
    <mini-banner />
    <maps />
    <services />
    <gallery />
    <myfooter />
  </div>
</template>

<script>
import IntroText from "../components/intro-text.vue";
import MiniBanner from "../components/mini-banner.vue";
import roofBanner from "../components/roof-banner.vue";
import Services from "../components/services.vue";
import Myfooter from "../components/myfooter.vue";
import CarouselBanner from "../components/carousel-banner.vue";
import Paint from "../components/paint.vue";
import Gallery from "../components/gallery.vue";
import Maps from "../components/maps.vue";

export default {
  name: "Home",

  components: {
    roofBanner,
    MiniBanner,
    IntroText,
    Services,
    Myfooter,
    CarouselBanner,
    Paint,
    Gallery,
    Maps,
  },
};
</script>

<style scoped>
#homepage {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 130px 0 0 0;
}
@media (max-width: 860px) {
  #homepage {
    padding: 150px 0 0 0;
  }
}
</style>
