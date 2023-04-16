<template>
    <div class="student-review mt-5 mb-5">
        <div class="container">
            <div class="main-head text-capitalize mb-5">
                Our Students Review
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
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-1.png" alt="">
            <h3>john deo</h3>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-2.png" alt="">
            <h3>john deo</h3>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-3.png" alt="">
            <h3>john deo</h3>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-4.png" alt="">
            <h3>john deo</h3>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-5.png" alt="">
            <h3>john deo</h3>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="student">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim animi atque numquam harum libero nemo, eligendi laboriosam beatae quo iure corrupti, neque rerum possimus non nisi quia! Cumque, tempora sit.</p>
            <img src="../assets/pic-6.png" alt="">
            <h3>john deo</h3>
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
    name:"StudentReview"
}
</script>

<style lang="scss">
    .student-review{

        .student{
            p {
                font-size: .95em;
                line-height: 2;
                color: #777;
                position: relative;
                background: #f0fdfa;
                border: 2px solid var(--green-color);
                margin-bottom: 20px;
                padding: 20px;
            }
            img{
                width: 70px;
                height: 70px;
                border-radius: 50%;
            }
            h3{
                margin-top: 15px;
                font-size: 1.5em;
            }
        }
        .swiper-slide{
        min-height: 60vh;
        cursor: grab;
        }

    }
</style>
