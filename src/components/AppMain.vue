<template>
  <main>
    <section class="jumbotron">
      <div class="container d-flex align-items-center">
        <div class="row-cols-12 text-center">
          <h1>Contemporary Ideas</h1>
          <p class="py-2">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ullam
            provident a non reprehenderit, repudiandae nobis et saepe tempora
            esse nihil quibusdam dignissimos voluptates consequuntur, assumenda
            corporis atque eius. Eum, non?
          </p>
          <button class="button-c mt-3">REGISTER NOW</button>
        </div>
      </div>
    </section>
    <section class="selection-application my-5">
      <div class="container-fluid">
        <div class="row text-center text-wrap justify-content-center">
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-1.png" alt="" />
            <h3 class="my-5">Languages</h3>
          </div>
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-2.png" alt="" />
            <h3 class="my-5">Software</h3>
          </div>
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-3.png" alt="" />
            <h3 class="my-5">Business</h3>
          </div>
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-4.png" alt="" />
            <h3 class="my-5">Chemistry</h3>
          </div>
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-5.png" alt="" />
            <h3 class="my-5">Science</h3>
          </div>
          <div class="container-application mx-2 py-5">
            <img src="../assets/img/h5-custom-icon-6.png" alt="" />
            <h3 class="my-5">DIY&Craft</h3>
          </div>
        </div>
      </div>
    </section>
    <section class="list-scroll-image my-5">
      <div class="text px-4">
        <h2 class="fw-bold fs-1 col-3">
          The Trusted Name for In-Home Tutoring.
        </h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ullam
          possimus ad, cumque, temporibus voluptates, laborum facilis obcaecati
          accusamus rerum eaque eum odio harum quasi neque deleniti nihil
          asperiores exercitationem quae.
        </p>
        <a href="">Learn More</a>
      </div>
      <div class="container-fluid">
        <div class="image row align-items-center px-3">
          <div class="col-11">
            <img src="../assets/img/h5-img-1.jpg" alt="" />
          </div>
          <div class="col-1">
            <div>
              <button class="button-t">
                <i class="fas fa-chevron-up"></i>
                <h2 class="fw-bold fs-5" href="">TOP</h2>
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="list-scroll-image-2 my-5">
      <div class="container-fluid">
        <div class="row align-items-center">
          <div class="col-6">
            <img src="../assets/img/h5-img-2.jpg" alt="" />
          </div>
          <div class="col-5">
            <h2 class="fw-bold">
              Empowering Childrento to Reach Their Potential
            </h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Reiciendis, voluptatem illo vero porro odit rem voluptates, omnis
              libero molestiae voluptatibus fugiat sunt explicabo fuga facere
              magnam rerum, officia ipsa cumque!
            </p>
            <div class="text row align-items-center">
              <div class="col-6 px-3">
                <span>168</span>
                <p class="px-2 fw-bold">User Stories</p>
              </div>
              <div class="col-6">
                <span>347</span>
                <p class="px-2 fw-bold">Events</p>
              </div>
            </div>
          </div>
          <div class="col-1 align-self-end">
            <div class="mt-3 position-absolute">
              <button class="button-t">
                <i class="fas fa-chevron-up"></i>
                <h2 class="fw-bold fs-5" href="">TOP</h2>
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="list-scroll-image-3 my-5">
      <div class="container d-flex align-items-center">
        <div class="text-center">
          <img src="../assets/img/testimonials-standard-2.png" />
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia
            repellat eum ipsum minima molestiae nesciunt, aliquam quaerat
            voluptates deleniti nulla dolores itaque consequatur debitis
            provident labore? Veritatis totam minima illo.
          </p>

          <h2>Joan Collins</h2>
          <p>STUDENT</p>
        </div>
      </div>
    </section>
    <AppSectionLearning />
    <AppSectionCourses />
    <AppSectionPricing />
    <AppLogo />
  </main>
</template>

<script>
import AppSectionLearning from "./AppSectionLearning.vue";
import AppSectionCourses from "./AppSectionCourses.vue";
import AppLogo from "./AppLogo.vue";
import AppSectionPricing from "./AppSectionPricing.vue";
export default {
  name: "AppMain",
  components: {
    AppSectionPricing,
    AppSectionCourses,
    AppLogo,
    AppSectionLearning,
  },
};
</script>

<style lang="scss" scoped>
main {
  .jumbotron {
    background-repeat: no-repeat;
    background-size: cover;
    background-image: url("../assets/img/h5-slide-3-background.jpg");
    .container {
      height: 92vh;
      color: white;
      p {
        font-size: 13px;
      }
      .button-c {
        background-color: #40c4ff;
        border: none;
        color: white;
        padding: 15px 32px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
      }
    }
  }

  .selection-application {
    height: 50vh;
    .container-application {
      height: 30vh;
      width: calc(90% / 6);
      background-color: #f2f8fc;
    }
    img {
      width: 38%;
    }
  }
  .list-scroll-image {
    // background-color: #40c4ff;
    .text {
      p {
        font-size: 21px;
      }
      a {
        color: #40c4ff;
      }
    }
  }
  .list-scroll-image-2 {
    // background-color: #40c4ff;
    h2 {
      font-size: 70px;
    }
    p {
      font-size: 23px;
    }
    .text {
      color: #40c4ff;
      span {
        font-size: 70px;
      }
      p {
        font-size: 25px;
      }
    }
  }
  img {
    width: 100%;
  }
  .button-t {
    background-color: #40c4ff;
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
  }
  .list-scroll-image-3 {
    background-image: url("../assets/img/h5-parallax-img-1.png");
    .container {
      img {
        width: 10%;
      }
      height: 80vh;
    }
  }
}
</style>
