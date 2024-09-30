<template>
  <section class="bg-yellow-100">
    <div class="p-4 md:p-8 lg:p-16">
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
          <Card
            blogImg="https://picsum.photos/1200/1200?random=49.jpg"
            chip="Innovation"
            title="best digital marketing stats we've seen this week"
            description="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eum, hic!"
            profile="https://picsum.photos/200/200?random=48.jpg"
            name="John Doe"
            day="22 days ago"
          />
        </swiper-slide>
        <swiper-slide>
          <Card
            blogImg="https://picsum.photos/1200/1200?random=50.jpg"
            chip="Technology"
            title="How AI is Revolutionizing the Tech Industry"
            description="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloribus, expedita!"
            profile="https://picsum.photos/200/200?random=47.jpg"
            name="Jane Smith"
            day="15 days ago"
          />
        </swiper-slide>

        <swiper-slide>
          <Card
            blogImg="https://picsum.photos/1200/1200?random=51.jpg"
            chip="Health"
            title="The Benefits of a Balanced Diet for Longevity"
            description="A balanced diet is essential for a healthy life. Learn the key components."
            profile="https://picsum.photos/200/200?random=46.jpg"
            name="Alex Brown"
            day="10 days ago"
          />
        </swiper-slide>

        <swiper-slide>
          <Card
            blogImg="https://picsum.photos/1200/1200?random=52.jpg"
            chip="Business"
            title="Top 10 Business Trends for 2024"
            description="Stay ahead of the curve with the latest business trends in 2024."
            profile="https://picsum.photos/200/200?random=45.jpg"
            name="Emily Clark"
            day="5 days ago"
          />
        </swiper-slide>

        <swiper-slide>
          <Card
            blogImg="https://picsum.photos/1200/1200?random=53.jpg"
            chip="Travel"
            title="Discover the Hidden Gems of Europe"
            description="Explore lesser-known destinations in Europe that will take your breath away."
            profile="https://picsum.photos/200/200?random=44.jpg"
            name="Michael Lee"
            day="3 days ago"
          />
        </swiper-slide>
      </swiper>
    </div>
  </section>
</template>

<script setup>
import { Pagination } from "swiper/modules";
import { Swiper, SwiperSlide } from "swiper/vue";
import Card from "./Cards.vue";
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
