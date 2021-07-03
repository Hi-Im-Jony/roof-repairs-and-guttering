<template>
  <div id="nav">
    <nav id="navbar">
      <a href="/"><img id="logo" src="../assets/logo4.png" alt=""/></a>

      <div v-if="windowWidth > 860" id="deets-container">
        <a class="deet" href="mailto:roofingr7@gmail.com">
          roofingr7@gmail.com
        </a>
        <a class="deet" href="tel:+353873794038">
          087 379 4038
        </a>
        <p>
          Dublin, Meath & Louth
        </p>
      </div>
      <div id="sticky-container" v-else>
        <sticky-mail />
        <sticky-phone />
      </div>
    </nav>
  </div>
</template>

<script>
import StickyMail from "./sticky-mail.vue";
import StickyPhone from "./sticky-phone.vue";
export default {
  name: "navbar",
  components: {
    StickyMail,
    StickyPhone,
  },
  data: () => ({
    windowWidth: window.innerWidth,
  }),
};
</script>

<style scoped>
#navbar {
  color: white;
  background: rgb(248, 248, 248);
  position: fixed;
  top: 0;
  z-index: 1;
  width: 100%;
  height: 130px;
  display: flex;
  padding: 0 50px 0 50px !important;
  justify-content: space-evenly;
  align-items: center;
  border-top: solid rgba(11, 19, 43, 0.836);
  border-width: 20px;
}
#logo {
  height: 100px;
  margin: 0 !important;
}
#deets-container {
  display: flex;
  align-items: center;
  font-size: 1.1rem;
}
.deet {
  color: rgb(202, 21, 21);
  padding: 10px;
  text-decoration: none;
}
.deet:hover {
  color: rgb(235, 37, 37);
}
p {
  color: rgb(202, 21, 21);
  padding: 10px;
  border-left: solid red;
  margin: 10px !important;
}
@media (max-width: 860px) {
  #navbar {
    flex-direction: column-reverse;
    padding: 0 !important;
    border: none;
    height: auto;
  }
  #sticky-container {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background: rgba(11, 19, 43, 0.836);
    padding: 10px 0 10px 0;
  }
}
</style>
