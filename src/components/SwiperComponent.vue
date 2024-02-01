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
            slide:[
                {
                    img : '04.jpg',
                    imgHover:'01.jpg',
                    title:'controller',
                    star:5,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '02.jpg',
                    imgHover:'04.jpg',
                    title:'controller',
                    star:5,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '05.jpg',
                    imgHover:'07.jpg',
                    title:'controller',
                    star:5,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '09.jpg',
                    imgHover:'08.jpg',
                    title:'controller',
                    star:4,
                    price:'$ 60',
                    priceUnderline:'$50'
                
                },
                {
                    img : '10.jpg',
                    imgHover:'11.jpg',
                    title:'controller',
                    star: 4 ,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '08.jpg',
                    imgHover:'02.jpg',
                    title:'Type',
                    star: 2 ,
                    price:'$ 70',
                    priceUnderline:'$50'
                },
                {
                    img : '04.jpg',
                    imgHover:'01.jpg',
                    title:'controller',
                    star:2,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '12.jpg',
                    imgHover:'14.jpg',
                    title:'controller',
                    star:1,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '15.jpg',
                    imgHover:'16.jpg',
                    title:'controller',
                    star:5,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '11.jpg',
                    imgHover:'12.jpg',
                    title:'controller',
                    star:4,
                    price:'$ 60',
                    priceUnderline:'$50'
                
                },
                {
                    img : '11.jpg',
                    imgHover:'17.jpg',
                    title:'controller',
                    star: 4 ,
                    price:'$ 60',
                    priceUnderline:'$50'
                },
                {
                    img : '01.jpg',
                    imgHover:'06.jpg',
                    title:'Type',
                    star: 2 ,
                    price:'$ 70',
                    priceUnderline:'$50'
                }
            ],
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
    :slidesPerView="4"
    :spaceBetween="30"
    :centeredSlides="true"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide class="product position-relative" v-for="(elem, i) in slide" :key="i">
        <div class="img-product">
            <img class="Sirv image-main" :src="getImagePath('../assets/'+ elem.img)" alt="">
            <img class="Sirv image-hover" :src="getImagePath('../assets/'+ elem.imgHover)" alt="">
        </div>
        <div class="info-product product-info position-absolute bottom-0 start-0">
            <div>
                <i  v-for="(ele,i) in elem.star" :key="i" class="fa-solid fa-star color-span"></i>
                <i v-for="(ele,i) in (5 - elem.star)" :key="i" class="fa-regular fa-star text-white"></i>
            </div>
            <h4 class="text-white">
                {{elem.title}}
            </h4>
            <div>
                <span class="text-decoration-line-through fs-2 text-white">
                    {{elem.priceUnderline}}
                </span>  
                <span class=" color-span fs-2"> 
                    {{elem.price}}
                </span>
            </div>
        </div>
    </swiper-slide>
  </swiper>
</template>

<style lang="scss" scoped>
.product{
    width: calc(100% / 4);
    .img-product{
        width: 100%;
        height: 200px;
        
        img{
            width: 100px;
            height: 100px;
            object-fit: cover;
        }
    }
    .img-product img.Sirv.image-hover{
        position: absolute;
        top: 0;
        right: 0;
        left: 0;
        bottom: 0;
        object-fit: contain;
        opacity: 0;
        transition: opacity .2s;
        
    }
    .img-product:hover img.Sirv.image-hover {
        opacity: 1;
     }
     .color-span{
        color: #F9AA01;
    }
}
</style>