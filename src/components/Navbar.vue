<!-- eslint-disable prettier/prettier -->
<template>
   <nav class="navbar navbar-expand-lg mb-5 navbar-light bg-light fixed-top">
    <div class="container">
        <router-link to="/" ><a class="navbar-brand text-capitalize" href="#"><fontAwesome icon="lightbulb" class="me-1"/>educa</a></router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
        <span class="navbar-toggler-icon"><fontAwesome icon="bars" /></span>
      </button>
      <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
        <div class="offcanvas-header">
          <h5 class="offcanvas-title text-capitalize" id="offcanvasNavbarLabel">educa</h5>
          <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
          <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
            <li class="nav-item" >
              <router-link to="/" ><a class="nav-link " @click="scroller()">Home</a></router-link> 
          </li>
          <li class="nav-item" >
              <router-link to="/about" ><a class="nav-link" @click="scroller()">About</a></router-link>
          </li>
          <li class="nav-item" >
              <router-link to="/courses" ><a class="nav-link " @click="scroller()">Courses</a></router-link>
          </li>
          <li class="nav-item" >
              <router-link to="/contact" ><a class="nav-link " @click="scroller()">Contact</a></router-link>
          </li>
          </ul>
          <form class="d-flex">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">Search</button>
          </form>
        </div>
      </div>
    </div>
  </nav>
</template>
<!-- eslint-disable prettier/prettier -->
<script>
    let navs=document.querySelectorAll(".nav-link");
export default {
    name:"AppHeader",
    el:".navbar",
    data:function(){
        return{
            navs:navs,
            scroller:function(){
                window.scrollTo(0,0)
            }
        }

    }
}
</script>
<!-- eslint-disable prettier/prettier -->
<style lang="scss" scoped>
    .navbar{
        z-index: 10000;
        .navbar-toggler-icon{
            background: none;
            font-size: 1.2em;
            width:fit-content;
            height: fit-content;
        }
        .nav-item a{
            text-decoration: none !important;
            font-weight: 400 !important;
            transition: .3s;
            :hover{
                color:var(--green-color) !important;
            }
        }
        .navbar-brand svg{
            color:var(--green-color) !important;
        }
        .navbar-toggler{
            border-color:transparent;
        }
        .navbar-toggler:focus {
            box-shadow: none;
        }
        .navbar-toggler[aria-expanded="true"] {
            border-color: transparent;
            
        }
    }
    
    @media (min-width:991px) {
        .navbar-brand{
            margin-right: 50%;
        }
    }
    

</style>