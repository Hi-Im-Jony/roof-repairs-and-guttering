<template>
  <div id="homepage">
    <roof-banner />
    <p id="intro-text">
      MJ Roofing Contractors offers the highest standard of roofing installation
      and roofing repair to clients in Dublin, Kildare, Wicklow and Meath.

      <br /><br />

      Our team of Dublin roofing experts have over 25 years of experience and
      complete every job to the very highest of regulatory standards.

      <br /><br />

      From pitched roofs to flat roofs, we have the expertise and experience to
      complete everything from small roofing repairs to complete roofing
      installations.

      <br /><br />

      We specialise in flat roof installations and flat roof repairs on home
      extensions. We can refit old, poorly laid flat roofs or install a flat
      roof on a new extension. Whatever the roofing requirement, clients can
      rest assured that their roofing service will be completed to the high MJ
      Roofing Contractors standard of quality and craftsmanship.

      <br /><br />

      All our roofing services come with a 25-year guarantee and are available
      with a free no-obligation quote.
    </p>
    <mini-banner />
  </div>
</template>

<script>
import MiniBanner from "../components/mini-banner.vue";
import roofBanner from "../components/roof-banner.vue";

export default {
  name: "Home",

  components: {
    roofBanner,
    MiniBanner,
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
#intro-text {
  width: 50%;
  margin: 30px 0 30px 0;
}
</style>
