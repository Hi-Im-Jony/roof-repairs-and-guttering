<template>
  <div id="homepage">
    <roof-banner />
    <intro-text />
    <mini-banner />
    <services />
    <media-tabs />
  </div>
</template>

<script>
import IntroText from "../components/intro-text.vue";
import MiniBanner from "../components/mini-banner.vue";
import roofBanner from "../components/roof-banner.vue";
import Services from "../components/services.vue";
import mediaTabs from "../components/media-tabs.vue";

export default {
  name: "Home",

  components: {
    roofBanner,
    MiniBanner,
    IntroText,
    Services,
    mediaTabs,
  },
};
</script>

<style scoped>
#homepage {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 50px 0 50px 0;
}
</style>
