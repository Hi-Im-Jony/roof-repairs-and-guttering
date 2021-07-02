<template>
  <div id="mini-banner">
    <div id="text-container">
      <p id="text">
        For a free no-obligation quote on your next flat roofing repair or
        pitched roof repair, get in contact with MJ Roofing Contractors today.
      </p>
      <phone-btn />
    </div>
    <div id="image-container">
      <img id="roofer" src="../assets/roofer.png" alt="" />
    </div>
  </div>
</template>
<script>
import phoneBtn from "./phone-btn.vue";
export default {
  components: { phoneBtn },
  name: "mini-banner",
};
</script>

<style scoped>
#mini-banner {
  background: rgb(34, 33, 33);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
#text-container {
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}
#text {
  width: 85%;
  font-size: 25px;
  margin: 0 0 60px 0;
}
#image-container {
  width: 50%;
}
#roofer {
  width: 100%;
}
</style>
