<template>
    <div class="expert-teacher mt-5 mb-5">
        <div class="container">
            <div class="main-head text-capitalize mb-5">
                Expert Teachers
            </div>
            <Swiper class="mb-5"
                :modules="modules"
                :breakpoints="swiperOptions.breakpoints"
                :loop="true"
                navigation
                :pagination="{ clickable: true }"
                :autoplay="{
                delay:5000,
                disableOnInteraction:false,
                }"
                
            >
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-1.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-2.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-3.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-4.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-5.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
            </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="teacher mb-4">
            <div class="teacher-image">
                <img src="../assets/teacher-6.png" alt="" class="img-">
                <div class="icons mt-4">
                    <fontAwesome :icon="['fab','facebook']" class="me-4" />
                    <fontAwesome :icon="['fab','twitter']" class="me-4" />
                    <fontAwesome :icon="['fab','instagram']" class="me-4" />
                    <fontAwesome :icon="['fab','linkedin']" class="me-4" />
                </div>
            </div>
            <div class="name mt-4 d-flex justify-content-between">
                <h3>john deo</h3>
                <span>expert tutor</span>
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
    name:"ExpertTeacher"
}
</script>

<style lang="scss">
    .expert-teacher{

        .swiper-slide{
        min-height: 40vh;
        cursor: grab;
    }
    .teacher{
        .teacher-image{
            position: relative;
            overflow: hidden;
            &:hover .icons{
                bottom: 0%;
            }
            .icons{
                position: absolute;
                bottom: -20%;
                width: 100%;
                padding: 10px;
                background-color: rgba($color: #000000, $alpha: .7);
                transition: .3s;
                svg{
                    padding: 0;
                    background-color: transparent;
                    font-size: 1.2em;
                    transition: .3s;
                    &:hover{
                        color:var(--green-color);
                        
                    }
                }
            }
            img{
                width: 100%;
                background-color: #f0fdfa;
                transition:.3s;
            }
            &:hover img{
                    background-color:var(--green-color) ;
                }
        }
    }
    .swiper-pagination{
        bottom: 0;
    }
    }
</style>