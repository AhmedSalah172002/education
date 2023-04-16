<template>
    
    <ContactLand />
    <GetTouch />
    <ContactForm />
    <QuestionLand />
    <AdLand />
    <FotterLand />
  </template>
  <!-- eslint-disable prettier/prettier -->
  
  <script>
import ContactLand from "@/components/ContactLand.vue";
import GetTouch from "@/components/GetTouch.vue";
import ContactForm from "@/components/ContactForm.vue";
import QuestionLand from "@/components/QuestionLand.vue";
import AdLand from "@/components/AdLand.vue";
import FotterLand from "@/components/FotterLand.vue";
  
  export default {
    name:"CoursesView",
    components:{
        ContactLand,
        GetTouch,
        ContactForm,
        QuestionLand,
        AdLand,
        FotterLand
    }
  }
  </script>
  