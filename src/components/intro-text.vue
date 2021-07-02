<template>
  <div id="container">
    <faq />
    <p id="intro-text">
      Here at Roofing Repairs & Guttering, we offer the highest standard of
      roofing installation and roofing repair to clients in Dublin, Meath and
      Louth.

      <br /><br />

      Our team of roofing experts have over 25 years of experience and complete
      every job to the very highest of regulatory standards.

      <br /><br />

      From pitched roofs to flat roofs, we have the expertise and experience to
      complete everything from small roofing repairs to complete roofing
      installations.

      <br /><br />

      We specialise in flat roof installations and flat roof repairs on home
      extensions. We can refit old, poorly laid flat roofs or install a flat
      roof on a new extension. Whatever the roofing requirement, clients can
      rest assured that their roofing service will be completed to our high
      standard of quality and craftsmanship.

      <br /><br />

      All our roofing services come with a 25-year guarantee and are available
      with a free no-obligation quote.
    </p>
    <quote-form />
  </div>
</template>

<script>
import faq from "./faq.vue";
import QuoteForm from "./quote-form.vue";
export default {
  name: "intro-text",
  components: {
    faq,
    QuoteForm,
  },
};
</script>

<style scoped>
#container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}
#intro-text {
  font-size: 20px;
  width: 40%;
  margin: 30px 20px 30px 20px;
}
#image {
  width: 25vw;
}
@media (max-width: 1100px) {
  #container {
    flex-direction: column;
  }
  #intro-text {
    width: 80%;
    text-align: center;
  }
}
</style>
