<template>
  <div id="homepage">
    <roof-banner />
    <intro-text />
    <mini-banner />
    <services />
  </div>
</template>

<script>
import IntroText from "../components/intro-text.vue";
import MiniBanner from "../components/mini-banner.vue";
import roofBanner from "../components/roof-banner.vue";
import Services from "../components/services.vue";

export default {
  name: "Home",

  components: {
    roofBanner,
    MiniBanner,
    IntroText,
    Services,
  },
};
</script>

<style scoped>
#homepage {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 50px;
}
</style>
