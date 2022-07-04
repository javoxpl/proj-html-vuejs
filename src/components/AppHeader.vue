<template>
  <header>
    <nav class="navbar navbar-expand position-absolute">
      <div class="container-fluid py-5 mx-5">
        <a class="navbar-brand" href="#">
          <img src="../assets/img/logo-light.png" alt="" />
        </a>
        <div>
          <ul class="navbar-nav">
            <li
              class="nav-item mx-5"
              v-for="(elm, index) in voces"
              :key="index"
            >
              <a href="#">{{ elm }}</a>
            </li>
            <li
              class="nav-item mx-5"
              v-for="(elmi, index) in icons"
              :key="index"
            >
              <i :class="`${elmi}`"></i>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      voces: ["HOME", "COURSES", "INSTRUCTORS", "EVENTS", "PAGES", "ELEMENTS"],
      icons: ["fas fa-search", "fas fa-shopping-bag", "fas fa-bars"],
    };
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 240px;
  height: 50px;
}
i {
  color: white;
  cursor: pointer;
}
</style>
