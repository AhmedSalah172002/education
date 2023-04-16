<template>
    <CoursesLand />
    <FamousCourses />
    <FotterLand />
  </template>
  <!-- eslint-disable prettier/prettier -->
  
  <script>
import CoursesLand from "@/components/CoursesLand.vue";
import FamousCourses from "@/components/FamousCourses.vue";
import FotterLand from "@/components/FotterLand.vue";
  
  export default {
    name:"CoursesView",
    components:{
        CoursesLand,
        FamousCourses,
        FotterLand
    }
  }
  </script>
  