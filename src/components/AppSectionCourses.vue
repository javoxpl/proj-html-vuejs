<template>
  <section>
    <div class="container-fluid my-5 px-5">
      <div class="text-center container my-5 justify-content-center">
        <h2>Popular Online Courses</h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Explicabo
          nostrum provident distinctio nam perferendis deleniti amet consectetur
          quidem eos nisi, quod ducimus, consequatur officiis rerum quasi,
          necessitatibus ullam vel! Modi.
        </p>
      </div>
      <div class="card_items row">
        <div class="box col-4" v-for="(elm, index) in cards" :key="index">
          <AppCard :element="elm"></AppCard>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import AppCard from "../components/AppCard.vue";
export default {
  name: "AppSectionCourses",
  components: {
    AppCard,
  },
  data() {
    return {
      cards: [
        {
          course: "Android Developer",
          picture: "course-5-f-img.jpg",
          teacher: "David Sanders",
          value: "FREE",
          description:
            "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.",
          type: "Programming",
        },
        {
          course: "Web Designing",
          picture: "course-6-f-img.jpg",
          teacher: "Jennifer Powell",
          value: "FREE",
          description:
            "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.",
          type: "Programming",
        },
        {
          course: "Financial Modelling",
          picture: "course-12-f-img.jpg",
          teacher: "Edward Bowman",
          value: "$20",
          description:
            "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.",
          type: "Business",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
