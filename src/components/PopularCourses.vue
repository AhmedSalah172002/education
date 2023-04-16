<template>
    <div class="Popular-Courses mt-5 mb-5">
        <div class="container">
            <div class="main-head text-capitalize mb-5">
                our popular courses
            </div>
            <Swiper class="mb-5"
                :modules="modules"
                :breakpoints="swiperOptions.breakpoints"
                :loop="true"
                navigation
                :pagination="{ clickable: true }"
                :autoplay="{
                delay:7000,
                disableOnInteraction:false,
                }"
                
            >
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-1.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-2.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-3.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-4.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-5.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="course text-capitalize">
            <div class="course-image mb-4">
                <img src="../assets/course-1-6.png" alt="" class="img-fluid" />
            </div>
            web development
            <div class="course-content">
               <h3>web development</h3>
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum, ratione?</p>
               <a href="#" class="btn1">read more</a>
            </div>
        </div>
      </swiper-slide>
    </swiper>
        </div>
    </div>
</template>

<script>
import  { Autoplay , Pagination } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'


import "swiper/css";
import "swiper/css/pagination";
export default {
    data () {
        return{
            swiperOptions: {
          breakpoints: {       
      320: {       
         slidesPerView: 1,
         spaceBetween: 10     
      },          
      767: {       
         slidesPerView: 2,       
         spaceBetween: 50     
      },   
  
      991: {       
         slidesPerView: 3,       
         spaceBetween: 30     
      } 
   }
}
        }
    },
    components: {
      Swiper,
      SwiperSlide
    },
    setup() {
      return {
        modules: [Autoplay,Pagination],
      }
    },
    name:"PopularCourses"
}
</script>

<style lang="scss">
    .Popular-Courses{
        .course{
            text-align: center;
            position: relative;
            background: #f0fdfa;
            overflow: hidden;
            margin-bottom: 80px;
            overflow: hidden;
            
            &:hover .course-content{
                bottom: 0;
            }
        }
        .swiper-slide{
        min-height: fit-content;
        cursor: grab;
    }
    .course-image{
        padding:2rem;
    }
    }
    .course-content{
        position: absolute;
        bottom:-100%; 
        right:0;
        left:0;
        transition: .3s;
        background-color: var(--green-color);
        color: white;
        padding: 15px 25px;
        p{
            color: #eee;
            line-height: 2;
        }
        .btn1{
                display: block;
                padding: 3px 10px;
                text-align:center;
                background-color:white ;
                color:var(--green-color) !important;
                margin: auto;
                text-transform: capitalize;
                border: 1px solid var(--green-color);
                width: fit-content;
                font-size: 1.3em;
            }
    }
</style>