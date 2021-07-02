<template>
  <div id="faq-container">
    <h1 style="text-align:center; color:#DC143C;">FAQ's</h1>
    <VueFaqAccordion :items="myItems" />
  </div>
</template>

<script>
import VueFaqAccordion from "vue-faq-accordion";

export default {
  components: {
    VueFaqAccordion,
  },
  data() {
    return {
      myItems: [
        {
          title: "How much is a flat roof repair?",
          value:
            "We offer free no-obligation quotes on all flat roof repairs. Our quotes are based on the type of flat roof and the nature of the repairs needed. No matter the specifics of your flat roof repair we always make every effort to supply a competitive quote.",
        },
        {
          title: "How long is a day and year on Venus?",
          value:
            "Venus takes 224.7 Earth days to complete one orbit around the Sun.",
        },
        {
          title: "What animal smells like popcorn?",
          value: "Binturongs smell like popcorn.",
        },
      ],
    };
  },
};
</script>

<style scoped>
#faq-container {
  width: 40vw;
}
@media (max-width: 800px) {
  #faq-container {
    width: 75vw;
  }
}
</style>
