<template>
  <div id="container">
    <h1>
      Gallery
    </h1>
    <v-tabs fixed-tabs background-color="#DC143C" color="white" dark>
      <v-tab>
        Tab 1
      </v-tab>

      <v-tab>
        Tab 2
      </v-tab>

      <v-tab-item class="tab-content">
        <tab-1 />
      </v-tab-item>
      <v-tab-item class="tab-content">
        <tab-2 />
      </v-tab-item>
    </v-tabs>
  </div>
</template>

<script>
import Tab1 from "./tab1.vue";
import Tab2 from "./tab2.vue";

export default {
  components: {
    Tab1,
    Tab2,
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
.grid {
  width: 100%;
  padding: 0 !important;
  margin: 0 auto !important;
  height: 50vh !important;
  overflow-y: scroll;
}
.grid-sizer,
.grid-item {
  width: 32%;
  min-width: 100px;
}
.grid-item img {
  padding: 5px;
  width: 100%;
}

@media (max-width: 660px) {
  #container {
    padding: 20px 10vw 20px 10vw;
  }
}
</style>
