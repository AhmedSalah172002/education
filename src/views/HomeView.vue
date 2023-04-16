<template>
  
    <HomeLand />
    <PopularSubject />
    <PopularCourses />
    <FotterLand />
</template>

<script>
// @ is an alias to /src
import HomeLand from '@/components/HomeLand.vue';
import PopularSubject from '@/components/PopularSubject.vue';
import PopularCourses from '@/components/PopularCourses.vue';
import FotterLand from '@/components/FotterLand.vue';


export default {
  name: 'HomeView',
  components: {
    HomeLand,
    PopularSubject,
    PopularCourses,
    FotterLand,
  }
}
</script>
