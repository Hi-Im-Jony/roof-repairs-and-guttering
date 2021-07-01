<template>
  <a id="phone-btn" href="tel:+353873794038">
    087 379 4038
  </a>
</template>

<script>
export default {
  name: "phone-btn",
};
</script>

<style scoped>
#phone-btn {
  color: white;
  text-decoration: none;
  background: rgb(185, 22, 22);
  padding: 10px;
  border: solid white;
  border-radius: 30px;
}
#phone-btn:hover {
  background: rgb(99, 36, 36);
}
</style>
