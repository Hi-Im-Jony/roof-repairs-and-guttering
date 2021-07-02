<template>
  <div id="homepage">
    <roof-banner />
    <intro-text />
    <mini-banner />
    <services />
    <media-tabs />
    <myfooter />
  </div>
</template>

<script>
import IntroText from "../components/intro-text.vue";
import MiniBanner from "../components/mini-banner.vue";
import roofBanner from "../components/roof-banner.vue";
import Services from "../components/services.vue";
import mediaTabs from "../components/media-tabs.vue";
import Myfooter from "../components/myfooter.vue";

export default {
  name: "Home",

  components: {
    roofBanner,
    MiniBanner,
    IntroText,
    Services,
    mediaTabs,
    Myfooter,
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
</style>
