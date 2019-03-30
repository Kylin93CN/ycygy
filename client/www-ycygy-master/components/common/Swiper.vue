<template>
  <div class="swiper swiperBox" v-swiper:swiper="swiperOption" ref="swiperBox" @mouseenter="stopSwiper" @mouseleave="startSwiper">
    <div class="swiper-wrapper">
      <div class="swiper-slide" v-for="(banner,index) in banners" :key="`banner${index}`">
        <img :src="banner">
      </div>
    </div>
    <div class="swiper-pagination"  slot="pagination"></div>
</div>
</template>

<script>
  export default {
    data(){
      return {
        // 所有配置均为可选（同Swiper配置）  
        banners: [ 
          '//shangzhibo-img.b0.upaiyun.com/client/user/105096/1553002788882/1553002787427_banner4.jpg',
          '//shangzhibo-img.b0.upaiyun.com/client/user/105096/1553002192918/1553002191460_banner3.jpg'
        ],
        swiperOption: {
          loop: true,
          speed: 500,
          grabCursor : true,
          effect : 'fade',
          notNextTick: true,
          slidesPerView: 'auto',
          centeredSlides: true,
          pagination: {
            el: '.swiper-pagination',
            clickable: true
          },
          on: {
            slideChange() {
            },
            tap() {
            }
          },
          autoplay: {
            delay: 3500,
            disableOnInteraction: false,
          },
          autoplayDisableOnInteraction:false,
          mousewheel: false,
          preloadImages: false,
          lazy: true
        }
      }
    },
    swiper() {
        // 如果你需要得到当前的swiper对象来做一些事情，你可以像下面这样定义一个方法属性来获取当前的swiper对象，同时notNextTick必须为true
        return this.$refs.swiperBox.swiper
    },
    methods:{
        stopSwiper(){
            this.swiper.autoplay.stop()
        },
        startSwiper(){
            this.swiper.autoplay.start()
        }
    }
}
</script>

<style lang="scss" scoped>
.swiper {
  width: 100%;
  height:400px;
  img {
    width: 100%;
    height: 400px;
  }
}
</style>