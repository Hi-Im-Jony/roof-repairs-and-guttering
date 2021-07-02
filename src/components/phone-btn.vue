<template>
  <a id="phone-btn" href="tel:+353873794038">
    <v-icon id="icon" dark>
      mdi-phone
    </v-icon>
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
  color: rgb(236, 241, 245);
  text-decoration: none;
  background: rgb(185, 22, 22);
  padding: 10px;
  border: solid rgb(236, 241, 245);
  border-width: 2px;
  border-radius: 30px;
  display: flex;
  align-items: center;
}
#phone-btn:hover {
  background: rgb(126, 52, 52);
}
#icon {
  margin-right: 15px;
}
</style>
