<template>
  <div id="imgs-container">
    <div class="img-container">
      <img src="../assets/roofs/roof1.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof2.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof3.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof4.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof5.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof6.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof7.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof8.jpeg" alt="" />
    </div>
    <div class="img-container">
      <img src="../assets/roofs/roof9.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "roofingImgs",
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
