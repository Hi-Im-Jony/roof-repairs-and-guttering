<template>
  <div id="imgs-container">
    <div class="img-container">
      <img src="../assets/gutters/gutter1.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/gutters/gutter2.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/gutters/gutter3.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "gutteringImgs",
};
</script>

<style scoped>
#imgs-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.img-container {
  width: 25vw;
  height: 25vw;
  max-width: 300px;
  max-height: 300px;
  margin: 5px;
  border-width: 1px;
}
img {
  object-fit: contain;
  width: inherit;
  height: inherit;
  max-width: inherit;
  max-height: inherit;
}
</style>
