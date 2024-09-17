<template>
  <section>
    <div class="p-4 md:p-8 lg:p-16 bg-gray-100 w-full flex flex-col md:flex-row bg-white">
      <!-- Text Section -->
      <div class="w-full md:w-1/2 flex flex-col justify-center space-y-6 mb-4 md:mb-0">
        <h2 class="text-2xl font-bold text-gray-800">This is a heading information</h2>
        <p class="text-body1 text-medium text-gray-400">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam tempore, suscipit vitae quaerat eum, vel corporis doloremque ullam quod nulla nobis provident. Eligendi, saepe natus dolorum maiores magni commodi accusantium?
        </p>
        <button class="shadow-indigo-200 py-2 px-6 text-white rounded-full bg-indigo-800" style="width: 200px;">
          Know More
        </button>
      </div>

      <!-- Swiper Section -->
      <div class="w-full md:w-1/2">
        <swiper
          :modules="[Pagination]"
          :pagination="{ clickable: true }"
          :breakpoints="{
            640: {
              slidesPerView: 1,
            },
            768: {
              slidesPerView: 2,
            },
            1024: {
              slidesPerView: 2,
            },
          }"
          class="swiper"
        >
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
          <swiper-slide>
            <ImgCard />
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import ImgCard from "./ImageCard.vue";
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  background-color: antiquewhite;
  height: 450px;
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
