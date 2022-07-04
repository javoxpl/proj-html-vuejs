<template>
  <section
    class="d-flex align-items-center justify-content-center container-fluid"
  >
    <div class="row row-cols-4">
      <div class="image" v-for="(elm, index) in images" :key="index">
        <img class="mx-5 px-4" :src="require('../assets/img/' + elm)" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppLogo",
  data() {
    return {
      images: [
        "h5-client-5.png",
        "h5-client-1.png",
        "h5-client-2.png",
        "h5-client-1.png",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container-fluid {
  height: 30vh;
  border-top: 1px solid gray;
}
img {
  width: 100%;
}
</style>
