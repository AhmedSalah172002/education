<!-- eslint-disable prettier/prettier -->
<template>
  <nav>
   <AppHeader />
  </nav>
  <router-view />
</template>
<!-- eslint-disable prettier/prettier -->
<script>
import AppHeader from "@/components/Navbar.vue";
export default {
  name:"App",
  components:{
    AppHeader,
  }
}
</script>
<!-- eslint-disable prettier/prettier -->

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
}

nav {
  a {
    font-weight: bold;

    &.router-link-exact-active {
      color:var(--green-color) !important;
    }
  }
}
</style>
