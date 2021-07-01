<template>
  <div id="roof-banner"></div>
</template>

<script>
export default {
  name: "roof-banner",
};
</script>

<style scoped>
#roof-banner {
  background-image: url("../assets/roof.jpg");
  background-attachment: fixed;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  position: absolute;
  height: 50vh;
  width: 100vw;
  padding: 0;
  margin: 0;
}
</style>
