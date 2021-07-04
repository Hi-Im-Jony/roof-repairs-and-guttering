<template>
  <div class="grid">
    <div class="grid-sizer"></div>
    <div class="grid-item">
      <img src="../assets/roofs/roof1.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof2.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof3.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof4.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof5.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof6.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof7.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof8.jpeg" alt="" />
    </div>
    <div class="grid-item">
      <img src="../assets/roofs/roof9.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
import Masonry from "masonry-layout";
window.onload = () => {
  const grid = document.querySelector(".grid");
  const masonry = new Masonry(grid, {
    itemSelector: ".grid-item",
    fitWidth: true,
  });
};
export default {
  name: "roofingImgs",
};
</script>

<style scoped>
.grid {
  width: 100%;
  padding: 0 !important;
  margin: 0 !important;
}
.grid-item {
  max-width: 30%;
  min-width: 100px;
}
.grid-item img {
  padding: 5px;
  width: 100%;
}
</style>
