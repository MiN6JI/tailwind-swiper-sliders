<template>
  <swiper :pagination="true" :modules="modules" class="mySwiper">
    <swiper-slide>
      <New />
    </swiper-slide>
    <swiper-slide>
      <New />
    </swiper-slide>
    <swiper-slide>
      <New />
    </swiper-slide>
    <swiper-slide>
      <New />
    </swiper-slide>
    <swiper-slide>
      <New />
    </swiper-slide>
    <swiper-slide>
      <New />
    </swiper-slide>
    </swiper>
</template>
<script setup>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import { Navigation } from 'swiper/modules';
  import { Pagination } from 'swiper/modules';
  import New from './News.vue'
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>