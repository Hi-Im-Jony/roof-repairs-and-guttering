<template>
  <stack :column-min-width="getWidth()" monitor-images-loaded class="stack">
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img1.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img2.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img1.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img2.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img1.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img2.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img1.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img2.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img2.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
    <stack-item style="transition: transform 300ms">
      <img src="../assets/img3.jpg" />
    </stack-item>
  </stack>
</template>

<script>
import { Stack, StackItem } from "vue-stack-grid";

export default {
  name: "tab2",
  components: {
    Stack,
    StackItem,
  },

  methods: {
    getWidth() {
      let w = 200;
      if (window.innerWidth < 255) {
        w = 80;
      } else if (window.innerWidth < 380) {
        w = 100;
      } else if (window.innerWidth < 500) {
        w = 150;
      }
      return w;
    },
  },
};
</script>
<style scoped>
.stack {
  width: 100% !important;
  padding: 0 10px 0 10px !important;
}

img {
  width: 100%;
  height: auto;
  padding: 5px;
}
</style>
