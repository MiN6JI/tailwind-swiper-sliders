<template>
  <section>
    <div class="p-4 md:p-8 lg:p-16 bg-gray-100">
      <swiper
        :modules="[Pagination]"
        :space-between="30"
        :pagination="{ clickable: true }"
        :breakpoints="{
          640: {
            slidesPerView: 1,
          },
          768: {
            slidesPerView: 2,
          },
          1024: {
            slidesPerView: 3,
          },
        }"
        class="swiper"
      >
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        <swiper-slide>
          <Testimonial />
        </swiper-slide>
        </swiper>
    </div>
  </section>
</template>

<script setup>
import { Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import Testimonial from "./testimonial.vue";
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  /* height: 250px; */
  text-align: center;
  font-size: 18px;
  background: #fff;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px;
  border-left: 7px rgb(117, 63, 255) solid;
  border-radius: 10px;

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
