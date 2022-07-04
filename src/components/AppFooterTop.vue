<template>
  <div class="container-fluid my-5">
    <nav class="row">
      <div class="d-flex flex-column col-3">
        <div>
          <img src="../assets/img/footer-logo-1.png" alt="logo" />
        </div>

        <ul>
          <li class="my-4" v-for="(elm, index) in todos" :key="index">
            <a href="#">{{ elm }}</a>
          </li>
        </ul>
        <div v-for="(elm, index) in infos" :key="index">
          <i :class="elm.icon"></i>
          <span>{{ elm.info }}</span>
        </div>
      </div>

      <div class="col-3">
        <h3>Popular Courses</h3>
        <ul>
          <li class="my-4" v-for="(elm, index) in courses" :key="index">
            <a href="#">{{ elm }}</a>
          </li>
        </ul>
      </div>

      <div class="col-3">
        <h3 class="fw-bold">Support</h3>
        <ul>
          <li class="my-4" v-for="(elm, index) in supports" :key="index">
            <a href="#">{{ elm }}</a>
          </li>
        </ul>
      </div>

      <div class="col-3">
        <h3>Flexible Learning</h3>
        <div class="logo">
          <img src="../assets/img/footer-img-1.png" alt="map" />
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "AppFooterTop",
  data() {
    return {
      todos: [
        "Providing Life Changing",
        "Experiences Through",
        "Education. Class That Fit Your",
        "Busy Life. Closer to Home",
      ],
      infos: [
        {
          info: "1-677-124-44227",
          icon: "fas fa-phone-alt",
        },

        {
          info: "Mon-Sat 8.00-18.00",
          icon: "far fa-clock",
        },
      ],
      courses: [
        "Business English",
        "Preston Marshall",
        "Social Computing",
        "David Sanders",
        "Learn Spanish",
        "Jennie King",
      ],
      supports: [
        "User dashboard",
        "Contact Us",
        "FAQ",
        "Course Offer",
        "Events",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
* {
  color: white;
}
li {
  color: grey;
}
.logo img {
  width: 100%;
}
</style>
