<template>
  <div id="paint-container">
    <img class="paint-img" src="../assets/fakro.jpeg" alt="" />
    <img class="paint-img" src="../assets/paint.jpeg" alt="" />
    <img class="paint-img" src="../assets/velux.jpeg" alt="" />
  </div>
</template>

<script>
export default {
  name: "paint",
};
</script>

<style scoped>
#paint-container {
  display: flex;
  width: 80%;
  justify-content: space-around;
  align-items: center;
  margin: 20px 0 20px 0;
}
.paint-img {
  width: 30vw;
  max-width: 400px;
  height: auto;
}
</style>
