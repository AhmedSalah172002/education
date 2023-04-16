<template>
    <div class="ad-land mt-5 mb-5">
        <div class="container">
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
       <img src="../assets/partner-logo-1.png" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/partner-logo-2.png" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/partner-logo-3.png" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/partner-logo-4.png" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="../assets/partner-logo-5.png" alt="">
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
         slidesPerView: 2,
         spaceBetween: 10     
      },          
      767: {       
         slidesPerView: 3,       
         spaceBetween: 50     
      },   
  
      991: {       
         slidesPerView: 5,       
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
    name:"AdLand"
}
</script>

<style lang="scss">
    .ad-land{
        .swiper-slide{
        min-height: 30vh;
        cursor: grab;
    }
    }
</style>