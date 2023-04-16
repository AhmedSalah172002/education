<template>
    <div class="home mt-5">
        <Swiper class="mb-5"
                :modules="modules"
                :slides-per-view="1"
                :loop="true"
                :space-between="50"
                navigation
                :pagination="{ clickable: true }"
                :autoplay="{
                delay:7000,
                disableOnInteraction:false,
                }"
                
            >
      <swiper-slide class="slide1">
        
            <div class="container">
                <div class="row">
                    <div class="col-lg-6">
                        <div class="content">
                            <h3>the best courses you will find find here!</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas impedit labore dolore unde, quidem corrupti?</p>
                            <a href="#" class="btn">get started</a>
                            </div>
                    </div>
                </div>
            </div>
        
      </swiper-slide>
      <swiper-slide class="slide2">
        <div class="container">
                <div class="row">
                    <div class="col-lg-6">
                        <div class="content">
                            <h3>the best courses you will find find here!</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas impedit labore dolore unde, quidem corrupti?</p>
                            <a href="#" class="btn">get started</a>
                            </div>
                    </div>
                </div>
            </div>
      </swiper-slide>
      <swiper-slide class="slide3">
        <div class="container">
                <div class="row">
                    <div class="col-lg-6">
                        <div class="content">
                            <h3>the best courses you will find find here!</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas impedit labore dolore unde, quidem corrupti?</p>
                            <a href="#" class="btn">get started</a>
                            </div>
                    </div>
                </div>
            </div>
      </swiper-slide>
    </swiper>
    </div>
  </template>
  
  <script>
import  { Autoplay , Pagination } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'


import "swiper/css";
import "swiper/css/pagination";
export default {
    components: {
      Swiper,
      SwiperSlide
    },
    setup() {
      return {
        modules: [Autoplay,Pagination]
      }
    },
    name:"HomeLand"
  }

</script>

<style lang="scss">
    .swiper-pagination-bullet-active{
        background-color: var(--green-color);
    }
    .swiper-pagination-bullet{
        background-color: var(--green-color);
    }
    .swiper-slide{
        min-height: 85vh;
        cursor: grab;
    }
    .swiper-button-next{
        background-color: white !important;
        color:white !important;
    }
    .slide1,.slide2,.slide3{
        background-repeat: no-repeat;
        background-size: cover !important;
      background-position: center !important;
        .content{
            color:white;
            text-align: left;
            margin-top:30%;
            line-height: 1.8;
            h3{
                text-transform: capitalize;
                font-size: 3em;

            }
            p{
                margin: 10px 0;
            }
            a{
                display: block;
                padding: 3px 10px;
                text-align:center;
                background-color: var(--green-color);
                    color:white !important;
                
                text-transform: capitalize;
                border: 1px solid var(--green-color);
                width: fit-content;
                font-size: 1.3em;
                transition: .3s;
                &:hover{
                    color:var(--green-color) !important;
                    background-color: transparent !important;
                }
            }
        }
    }
    .slide1{
        background: url(../assets/home-slide-1.jpg) ;
        
    }
    .slide2{
        background: url(../assets/home-slide-2.jpg) ;
    }
    .slide3{
        background: url(../assets/home-slide-3.jpg) ;
    }
    @media (max-width:767px) {
        .slide1 .content,.slide2 .content, .slide3 .content{
            margin-top:50%
        }
        .slide1 .content h3,.slide2 .content h3,.slide3 .content h3{
            font-size: 2em;
        }
        
    }
</style>