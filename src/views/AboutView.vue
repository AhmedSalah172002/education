<template>
  <AboutLand />
  <AboutDes />
  <ExpertTeacher />
  <StudentReview />
  <FotterLand />
</template>
<!-- eslint-disable prettier/prettier -->

<script>
import AboutLand from "@/components/AboutLand.vue";
import AboutDes from "@/components/AboutDes.vue";
import ExpertTeacher from "@/components/ExpertTeacher.vue";
import StudentReview from "@/components/StudentReview.vue";
import FotterLand from "@/components/FotterLand.vue";

export default {
  name:"AboutView",
  components:{
    AboutLand,
    AboutDes,
    ExpertTeacher,
    StudentReview,
    FotterLand
  }
}
</script>
