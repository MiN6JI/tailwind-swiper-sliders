<template>
  <section>
    <div
      class="p-4 md:p-8 lg:p-16 bg-gray-100 w-full flex flex-col md:flex-row"
    >
      <div
        class="w-full md:w-1/2 flex flex-col justify-center space-y-6 mb-4 md:mb-0"
      >
        <h2 class="text-3xl font-bold text-gray-800">
          Unlock Your Potential with Expert Guidance and Achieve Success Beyond
          Limits
        </h2>
        <p class="text-medium text-gray-700">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam
          tempore, suscipit vitae quaerat eum, vel corporis doloremque ullam
          quod nulla nobis provident. Eligendi, saepe natus dolorum maiores
          magni commodi accusantium?
        </p>
        <router-link
          class="underline underline-offset-4 uppercase font-bold text-red-500"
        >
          Know More
        </router-link>
      </div>

      <div class="w-full md:w-1/2">
        <swiper
          :modules="[Navigation]"
          :navigation="true"
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
            <ImgCard
              heading="Explore the Wonders of Nature"
              paragraph="Experience breathtaking landscapes and immerse yourself in the beauty."
              image="https://picsum.photos/500/768/?random=1&grayscale"
            />
          </swiper-slide>
          <swiper-slide>
            <ImgCard
              heading="Culinary Adventures Await"
              paragraph="Join us on a journey to discover delicious flavors and unique dishes from around the world."
              image="https://picsum.photos/500/768/?random=2"
            />
          </swiper-slide>
          <swiper-slide>
            <ImgCard
              heading="Embrace a Healthy Lifestyle"
              paragraph="Discover tips and tricks to lead a healthier, happier life through balanced nutrition and fitness."
              image="https://picsum.photos/500/768/?random=3&grayscale"
            />
          </swiper-slide>
          <swiper-slide>
            <ImgCard
              heading="Unlock Your Creative Potential"
              paragraph="Dive into the world of art and expression, and unleash your creativity with various techniques and mediums."
              image="https://picsum.photos/500/768/?random=4"
            />
          </swiper-slide>
          <swiper-slide>
            <ImgCard
              heading="Travel the World"
              paragraph="Explore diverse cultures, stunning landscapes, and unforgettable experiences across the globe."
              image="https://picsum.photos/500/768/?random=5&grayscale"
            />
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Navigation } from "swiper/modules";
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

.swiper-button-prev, .swiper-button-next{
  color: white;
  font-size: 20px;
  
}
.swiper-button-prev:after, .swiper-button-next:after{
  color: white;
  font-size: 20px;
}
</style>
