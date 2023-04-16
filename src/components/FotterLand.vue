<template>
    <div class="footer">
        <!-- Footer -->
<footer class="text-center text-lg-start  text-muted">
  <!-- Section: Social media -->

  <!-- Section: Social media -->

  <!-- Section: Links  -->
  <section class="">
    <div class="container text-center text-md-start mt-5">
      <!-- Grid row -->
      <div class="row mt-3">
        <!-- Grid column -->
        <div class="col-md-3 col-lg-4 col-xl-3 mx-auto mb-4">
          <!-- Content -->
          <h6 class="text-uppercase fw-bold mb-4">
            <router-link to="/" ><a class="navbar-brand text-capitalize" href="#"><fontAwesome icon="lightbulb" class="me-1"/>educa</a></router-link>
          </h6>
          <p >
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi, voluptatem.
          </p>
          <div class="icons mt-4">
              <fontAwesome :icon="['fab','facebook']" class="me-2 mb-3" />
              <fontAwesome :icon="['fab','twitter']" class="me-2 mb-3" />
              <fontAwesome :icon="['fab','instagram']" class="me-2 mb-3" />
              <fontAwesome :icon="['fab','whatsapp']" class="me-2 mb-3" />
          </div>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4">
          <!-- Links -->
          <h6 class="text-uppercase fw-bold mb-4">
            Quick Links
          </h6>
          <p>
            <router-link to="/" ><a class="nav-link ">Home</a></router-link> 
          </p>
          <p>
            <router-link to="/about" ><a class="nav-link">About</a></router-link>
          </p>
          <p>
            <router-link to="/courses" ><a class="nav-link ">Courses</a></router-link>
          </p>
          <p>
            <router-link to="/contact" ><a class="nav-link ">Contact</a></router-link>
          </p>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-3 col-lg-2 col-xl-2 mx-auto mb-4">
          <!-- Links -->
          <h6 class="text-uppercase fw-bold mb-4">
            Useful Links
          </h6>
          <p>
            <a href="#" class="link">help center</a>
          </p>
          <p>
            <a href="#" class="link">ask questions</a>
          </p>
          <p>
            <a href="#" class="link">send feedback</a>
          </p>
          <p>
            <a href="#" class="link">private policy</a>
          </p>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-4 col-lg-3 col-xl-3 mx-auto mb-md-0 mb-4">
          <!-- Links -->
          <h6 class="text-uppercase fw-bold mb-4">Contact</h6>
          <p><fontAwesome icon="home" class="me-3"/> Shobra,El Menoufia,Egypt</p>
          <p>
            <fontAwesome icon="envelope" class="me-3"/>
            ahmed123salah@gmail.com
          </p>
          <p><fontAwesome icon="phone" class="me-3"/> +20 1095572350</p>
          <p><fontAwesome icon="phone" class="me-3" /> +20 1553629437</p>
        </div>
        <!-- Grid column -->
      </div>
      <!-- Grid row -->
    </div>
  </section>
  <!-- Section: Links  -->

  <!-- Copyright -->
  <div class="container">
    <div class="text-center p-4" style="background-color: #f0fdfa;border-top: 1px solid var(--green-color);">
    © 2022 Copyright:
    <a class="text-reset fw-bold" href="https://github.com/ahmedsalah2002">Ahmed Salah</a>
  </div>
  </div>
  <!-- Copyright -->
</footer>
<!-- Footer -->
    </div>
</template>
<script>
export default {
    name:"FotterLand"
}
</script>
<style lang="scss">
    .footer{
      padding-top: 15px;
      .navbar-brand{
        font-size: 1.5em;
        svg{
            color:var(--green-color) !important;
        }
      }
     
        .link{
          text-transform: capitalize;
          color: #777 !important;
          line-height: 2;
          &:hover{
            color:var(--green-color) !important;
          }
        }
        .nav-link{
          color: #777 !important;
          line-height: 2;
          &:hover{
            color:var(--green-color) !important;
          }
        }
        h6{
            color: black;
        }
        background-color: #f0fdfa !important;
        
        a{
            color:black !important;
            text-decoration: none;
        }
    }
    .icons{
      font-size: 1.5em;
      svg{
        padding:  10px;
        background-color:var(--green-color) ;
        color: white;
        cursor: pointer;
        transition: .3s;
        &:hover{
          background-color:gray ;
        }
      }
    }
    
</style>