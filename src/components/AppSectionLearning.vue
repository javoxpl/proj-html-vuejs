<template>
  <section class="continer-fluid px-5">
    <div class="row">
      <ul class="col-3 list">
        <li class="py-4 px-5" v-for="(elm, index) in programs" :key="index">
          {{ elm }}
        </li>
      </ul>
      <div class="col-9">
        <div class="text">
          <h2>Learning Possibilities</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus illum
            quaerat, magni ut quisquam assumenda eligendi in ipsam asperiores
            consequuntur nihil dolorem optio, quo vitae. Pariatur similique est
            laboriosam suscipit.
          </p>
        </div>
        <div class="py-5 px-5 d-flex">
          <div class="py-5">
            <div v-for="(elm, index) in actions" :key="index">
              <p class="pt-3"><i class="fas fa-check"></i> {{ elm }}</p>
            </div>
          </div>
          <div class="image d-flex flex-column">
            <img src="../assets/img/h12-tabs-icon-1.png" alt="img" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionLearning",
  data() {
    return {
      programs: [
        "What We Do",
        "Degree Programme",
        "Carrer Archievements",
        "Personal Managment",
        "Steps To Success",
        "Knowledge Transfer",
      ],
      actions: [
        "We enrich lives throught learning.",
        "Maximizin potential throught individual attention.",
        "The trusted name.",
        "People teach. People learn. This is where they connect.",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.list {
  li {
    border: 1px solid grey;
    &:hover {
      border-left: 5px solid #40c4ff;
      color: #40c4ff;
      background-color: #f2f2f2;
    }
  }
}
</style>
