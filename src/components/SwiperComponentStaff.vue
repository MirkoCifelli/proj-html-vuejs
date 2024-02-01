<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';

  

  // import required modules
  import { Pagination } from 'swiper/modules';

  export default {
    data(){
        return{
            
            
        }
    },
    components: {
      Swiper,
      SwiperSlide,
    },
    methods:{
        getImagePath: function(imgPath){
                return new URL(imgPath, import.meta.url).href;
            },
  },
    setup() {
      return {
        modules: [Pagination],
      };
    },
  };
</script>


<template>
   <swiper
    :spaceBetween="30"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
        
            <div class="container d-flex flex-wrap justify-content-center p-5">
                <div class="img-staff position-relative">
                    <img src="../assets/t5-1-100x100_left.jpg" alt="">
                </div>
                <div class="absolute-quote">
                    <img src="../assets/quote.png" alt="">
                </div>
                <div class="staff-info d-flex flex-wrap align-items-center justify-content-center text-white">
                    <h4 class=" m-1">Lules Charls</h4><span class="orange">(Web designer)</span>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore harum iste ratione fuga adipisci repudiandae aut aperiam quae dolor explicabo omnis, recusandae vel totam quasi? Nemo rem laborum aperiam unde!
                    </p>
                </div>
            </div>
        
    </swiper-slide>
    <swiper-slide class="ms-2">
        <div class="container d-flex flex-wrap justify-content-center p-5 margin">
                <div class="img-staff position-relative">
                    <img src="../assets/t4-1-100x100_left.jpg" alt="">
                </div>
                <div class="absolute-quote">
                    <img src="../assets/quote.png" alt="">
                </div>
                <div class="staff-info d-flex flex-wrap align-items-center justify-content-center text-white">
                    <h4 class=" m-1">Din Desuza</h4><span class="orange">(Iphone Developer)</span>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore harum iste ratione fuga adipisci repudiandae aut aperiam quae dolor explicabo omnis, recusandae vel totam quasi? Nemo rem laborum aperiam unde!
                    </p>
                </div>
            </div>
    </swiper-slide>
    <swiper-slide class="ms-3">
        <div class="container d-flex flex-wrap justify-content-center p-5 margin">
                <div class="img-staff position-relative">
                    <img src="../assets/t2-1-100x100_left.jpg" alt="">
                </div>
                <div class="absolute-quote">
                    <img src="../assets/quote.png" alt="">
                </div>
                <div class="staff-info d-flex flex-wrap align-items-center justify-content-center text-white">
                    <h4 class=" m-1">Din Desuza</h4><span class="orange">(Iphone Developer)</span>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore harum iste ratione fuga adipisci repudiandae aut aperiam quae dolor explicabo omnis, recusandae vel totam quasi? Nemo rem laborum aperiam unde!
                    </p>
                </div>
            </div>
    </swiper-slide>
   
  </swiper> 
</template>

<style lang="scss" scoped>
.swiper {
  width: 140%;
  height: 100%;
    .swiper-slide {
    text-align: center;
    font-size: 18px;
    margin-left: -300px;
    }
    .swiper-slide img {
     display: block;
     width: 100%;
     height: 100%;
     object-fit: cover;
     
     
}
}
.orange{
        color:#F9AA01 ;
     }
     .img-staff{
            width: 100px;
            height: 100px;
            img{
                width: 100%;
                height: 100%;
                border-radius: 50%;
                border: 1px solid #F9AA01;
            }
            }
            .absolute-quote{
                position: absolute;
                left: 48%;
                background-color: #F9AA01;
                height: 20px;
                width: 20px;
                border-radius: 50%;
                line-height: 1;
               
            } 
              
</style>