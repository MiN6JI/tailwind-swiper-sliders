<template>
  <section>
    <div class="p-4 md:p-8 lg:p-16 bg-indigo-100">
      <swiper :pagination="true" :modules="modules" class="mySwiper">
        <swiper-slide>
          <New
            image="https://picsum.photos/800/800?random=50.jpg"
            title="Good News"
            day="22 July, 2024"
            textTitle="Every Point of View is different"
            description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. A, similique dignissimos culpa eius facilis veniam unde. Dignissimos doloribus alias tenetur."
            profileImg="https://picsum.photos/800/800?random=51.jpg"
            profileName="John Doe"
          />
        </swiper-slide>
        <swiper-slide>
          <New
            image="https://picsum.photos/800/800?random=52.jpg"
            title="Breaking News"
            day="15 August, 2024"
            textTitle="Understanding Different Perspectives"
            description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Voluptatum, dignissimos culpa eius!"
            profileImg="https://picsum.photos/800/800?random=53.jpg"
            profileName="Jane Smith"
          />
        </swiper-slide>
        <swiper-slide>
          <New
            image="https://picsum.photos/800/800?random=54.jpg"
            title="Latest Update"
            day="10 September, 2024"
            textTitle="Innovation in Action"
            description="Nunc nec justo libero. Sed a ante non lorem egestas commodo eget vel metus."
            profileImg="https://picsum.photos/800/800?random=55.jpg"
            profileName="Michael Johnson"
          />
        </swiper-slide>
        <swiper-slide>
          <New
            image="https://picsum.photos/800/800?random=56.jpg"
            title="New Discovery"
            day="1 October, 2024"
            textTitle="A Fresh Perspective"
            description="Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip."
            profileImg="https://picsum.photos/800/800?random=57.jpg"
            profileName="Emily Davis"
          />
        </swiper-slide>
      </swiper>
    </div>
  </section>
</template>
<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";
import { Pagination } from "swiper/modules";
import New from "./News.vue";
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
