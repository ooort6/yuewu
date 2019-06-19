<template>
  <div class="success_sh">
       <div class="swiper-container">
    <div class="swiper-wrapper">
     <img class="swiper-slide" src="../../../static/images/sh1.png" alt="">
     <img class="swiper-slide" src="../../../static/images/sh2.jpg" alt="">
         <img class="swiper-slide" src="../../../static/images/sh3.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh4.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh5.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh6.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh7.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh8.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh9.jpg" alt="">
     <img class="swiper-slide" src="../../../static/images/sh10.jpg" alt="">



    </div>
    <!-- Add Pagination -->
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
    <!-- <div class="swiper-pagination"></div> -->
  </div>
  <div class="success_2"></div>
       <img class="success_1" src="../../../static/images/sh.png" alt="">
  </div>
</template>
<script>
import Swiper from 'swiper';
export default {
    name:'success_sh',
    data() {
    return {
     
    };
  },
  mounted(){
new Swiper('.swiper-container', {
      effect: 'coverflow',
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      initialSlide :0,
      loop : true,
      grabCursor: true,
      centeredSlides: true,
      slidesPerView: "auto",
      coverflowEffect: {
        rotate: 0,
        stretch: 0,
        depth: 100,
        modifier: 1,
        // slideShadows : true,
      },
      // pagination: {
      //   el: '.swiper-pagination',
      // },
    });      
  },

}
</script>
<style lang="scss" scoped>
 .swiper-container {
      width: 61%;
      margin-bottom: 60px;
    }
    .swiper-slide {
      background-position: center;
      background-size: cover;
      width: 402px;
      height: 263px;
 
    }
    .swiper-button-next{
     background:url('../../../static/images/shright.png') no-repeat;
    }
    .swiper-button-prev{
     background:url('../../../static/images/shleft.png') no-repeat;

    }
  .success_sh{
      padding-top: 5%;
       height: 100%;
      background: url('../../../static/images/sh.jpg') no-repeat;
        // height: 100%;
        // width: 200px;
        // background: red;
        //  img{
        //         width: 100%;
        //     }
        .success_1{
            margin-top: 120px;
            display: block;
            margin:0 auto;
            margin-bottom: 145px;
        }
        .success_2{
            width:1230px;
            height:2px;
            background:rgba(115,115,115,1);
            margin:0 auto;
      margin-bottom: 60px;

        }
  }
</style>

