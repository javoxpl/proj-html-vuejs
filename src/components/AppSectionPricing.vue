<template>
  <div class="container-fluid my-5 px-5">
    <div class="text-center d-flex flex-column my-5">
      <h2 class="fw-bold fs-1">Pricing Plans</h2>
      <p class="fs-2">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptate
        quasi ipsum.
      </p>
    </div>
    <div class="row">
      <div class="col-3 list">
        <div class="box d-flex">
          <h3 class="px-5 py-5 fs-1">Save up to 40% by paying weekly</h3>
        </div>
        <ul>
          <li class="classes" v-for="(elm, index) in indicator" :key="index">
            {{ elm }}
          </li>
        </ul>
      </div>

      <div class="col-3 list">
        <div class="box box_image d-flex flex-column">
          <div class="image">
            <img src="../assets/img/h5-custom-icon-7.png" alt="" />
          </div>
          <div class="type">Standard</div>
          <div class="cost">$12</div>
        </div>
        <ul>
          <li>2</li>
          <li>15 DAYS</li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li>
            <div class="button">
              <button>GET IT NOW</button>
            </div>
          </li>
        </ul>
      </div>

      <div class="col-3 list">
        <div class="box box_image d-flex flex-column">
          <div class="image">
            <img src="../assets/img/h5-custom-icon-8.png" alt="" />
          </div>
          <div class="type">Professional</div>
          <div class="cost">$59</div>
        </div>
        <ul>
          <li>4</li>
          <li>30 DAYS</li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li><i class="fas fa-times"></i></li>
          <li>
            <div class="button">
              <button>GET IT NOW</button>
            </div>
          </li>
        </ul>
      </div>

      <div class="col-3 list">
        <div class="box box_image d-flex flex-column">
          <div class="image">
            <img src="../assets/img/h5-custom-icon-9.png" alt="" />
          </div>
          <div class="type">Advance</div>
          <div class="cost">$88</div>
        </div>
        <ul>
          <li>6</li>
          <li>30 DAYS</li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li><i class="fas fa-check"></i></li>
          <li>
            <div class="button">
              <button>GET IT NOW</button>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppSectionPricing",
  data() {
    return {
      indicator: [
        "Numbers of Course",
        "Time",
        "Web Designing",
        "Human-Centered Design",
        "Basik Marketing",
        "Phyton for Everybody",
        "Android Developer",
        "Business English",
      ],
      standard: false,
      proifessional: false,
      advance: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.row {
  background-color: white;
  .list {
    padding: 0px;
    &:hover .box_image {
      border-top-color: #40c4ff;
    }
  }
}
.box {
  min-height: 130px;
  border: 1px solid #efefef;
  border-top: 3px solid #d6f2ff;
}
li {
  text-align: center;
  line-height: 50px;
  border: 1px solid #efefef;
  .fa-check {
    color: #40c4ff;
  }
  .fa-times {
    color: #8f8f8f;
  }
}
.box_image {
  text-align: center;
  justify-content: center;
  background-color: #f7fdff;
  font-size: 20px;
  font-weight: 700;
}
.button {
  text-align: center;
  padding: 30px;
  background-color: #f7fdff;
  button {
    width: 100%;
    height: 60px;
    color: #8e8e8e;
    font-weight: 700;
    background-color: white;
    border: 1px solid #efefef;
    &:hover {
      color: white;
      background-color: #40c4ff;
    }
  }
}
</style>
