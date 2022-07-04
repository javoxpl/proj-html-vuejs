<template>
  <div class="container-fluid mt-5 d-flex justify-content-between">
    <div>Copyrights 2017 <i class="far fa-copyright"></i> Mikado Themes</div>
    <div class="d-flex px-5">
      <div>CALL +44 300 303 0266</div>
      <div class="social">
        <span>FOLLOW US</span>
        <a class="mx-3" href="#" v-for="(elm, index) in socials" :key="index">
          <i :class="elm"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooterBottom",
  data() {
    return {
      socials: ["fab fa-twitter", "fab fa-instagram", "fab fa-facebook"],
    };
  },
};
</script>

<style lang="scss" scoped></style>
