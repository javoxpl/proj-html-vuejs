<template>
  <footer>
    <div class="container-fluid pt-4">
      <AppFooterTop></AppFooterTop>
      <AppFooterBottom></AppFooterBottom>
    </div>
  </footer>
</template>

<script>
import AppFooterTop from "./AppFooterTop.vue";
import AppFooterBottom from "./AppFooterBottom.vue";
export default {
  name: "AppFooter",
  components: {
    AppFooterTop,
    AppFooterBottom,
  },
};
</script>

<style lang="scss" scoped>
footer {
  color: #b9b9b9;
  background-color: #222222;
}
</style>
