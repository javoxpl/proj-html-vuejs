<template>
  <div class="box">
    <div class="top">
      <div class="image">
        <img :src="require('../assets/img/' + element.picture)" alt="img" />
      </div>
      <div class="info d-flex">
        <div class="text">
          <h4>{{ element.course }}</h4>
          <h5>{{ element.teacher }}</h5>
        </div>
        <div class="price">
          <div :class="element.value == 'FREE' ? 'free' : 'pay'">
            {{ element.value }}
          </div>
        </div>
      </div>
    </div>
    <div class="bottom">
      <p>{{ element.description }}</p>
      <div>
        <span><i class="fas fa-user"></i> 1 </span>
        <span><i class="fas fa-tag"></i> {{ element.type }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppCard",
  props: {
    element: Object,
  },
};
</script>

<style lang="scss" scoped>
.box {
  color: #a6a6a6;
  border: 2px solid #f2f2f2;
  background-color: #fff;
  img {
    width: 100%;
  }
  .info {
    justify-content: space-between;
    h4 {
      color: black;
    }
    .price {
      padding: 2px;
      div {
        padding: 8px 20px;
        border-radius: 15px;
        font-size: 12px;
        color: white;
      }
    }
  }
  .info,
  .bottom {
    padding: 10px;
  }
  p {
    color: #a6a6a6;
  }
  .bottom span {
    margin-right: 8px;
  }
}
.free {
  background-color: #ffd740;
}
.pay {
  background-color: #40c4ff;
}
</style>
