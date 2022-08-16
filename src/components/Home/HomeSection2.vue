<template>
  <div class="Section2 mt-5 mt-md-4 mb-5">
    <h4 class="title mb-1">المتاجر المميزة</h4>
    <swiper
      :slides-per-view="8"
      :space-between="20"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
      :pagination="{ clickable: true }"
      :autoplay="{ delay: 5000 }"
      grabCursor
      loop="true"
      :navigation="{
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      }"
      :breakpoints="{
        200: {
          slidesPerView: 2,
        },
        400: {
          slidesPerView: 3,
        },
        600: {
          slidesPerView: 4,
        },
        800: {
          slidesPerView: 6,
        },
        1000: {
          slidesPerView: 8,
        },
      }"
    >
      <swiper-slide>
        <img src="../../assets/home/swiper1.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper2.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper3.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper4.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper5.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper6.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper1.png" alt="swiper1"
      /></swiper-slide>
      <swiper-slide>
        <img src="../../assets/home/swiper2.png" alt="swiper1"
      /></swiper-slide>
    </swiper>
    <div class="swiper-button-prev">
      <img src="../../assets/next.png" alt="next" />
    </div>
    <div class="swiper-button-next">
      <img src="../../assets/prev.png" alt="prev" />
    </div>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import swiperCore, {
  Navigation,
  Pagination,
  Scrollbar,
  A11y,
  Autoplay,
} from "swiper";

// Import Swiper styles
import "swiper/css/navigation";
import "swiper/css/pagination";
import "swiper/css/scrollbar";
swiperCore.use([Navigation, Pagination, Scrollbar, A11y, Autoplay]);
import "swiper/scss";
export default {
  name: "HomeSection2",
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>
<style lang="scss" scoped>
.swiper-button-prev::after,
.swiper-button-next::after {
  display: none;
}
.swiper-button-prev img,
.swiper-button-next img {
  width: 10px;
}
.Section2 {
  position: relative;
}
.swiper-slide img {
  width: 100%;
}
.swiper {
  width: 90%;
  height: 110px;
}
@media (max-width: 576px) {
  .swiper {
    height: 140px;
  }
}
</style>
<style>
.swiper-button-next,
.swiper-button-prev {
  top: 50% !important;
}
.swiper-pagination-bullet {
  width: 17px;
  height: 17px;
  background: #fff;
  border: 2px solid rgba(58, 194, 203, 1);
}
.swiper-pagination-bullet-active {
  position: relative;
}
.swiper-pagination-bullet-active::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  width: 7px;
  border-radius: 50%;
  height: 7px;
  transform: translate(-50%, -50%);
  background: rgba(58, 194, 203, 1);
}
</style>
