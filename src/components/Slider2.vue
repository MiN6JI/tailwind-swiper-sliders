<template>
  <section>
    <div class="p-4 md:p-8 lg:p-16 bg-gray-100">
      <swiper
        :modules="[Pagination]"
        :space-between="30"
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
          <Testimonial
            name="John Doe"
            profession="Software Engineer"
            image="https://picsum.photos/200/200?random=3.jpg"
            title="Climate Standard"
            description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur, tenetur?"
          />
        </swiper-slide>
        <swiper-slide>
          <Testimonial
            name="Jane Smith"
            profession="Marketing Specialist"
            image="https://picsum.photos/200/200?random=4.jpg"
            title="Amazing Service"
            description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quibusdam, assumenda?"
          />
        </swiper-slide>
        <swiper-slide>
          <Testimonial
            name="Michael Johnson"
            profession="Graphic Designer"
            image="https://picsum.photos/200/200?random=5.jpg"
            title="Highly Recommended"
            description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium."
          />
        </swiper-slide>
        <swiper-slide>
          <Testimonial
            name="Emily Davis"
            profession="Project Manager"
            image="https://picsum.photos/200/200?random=6.jpg"
            title="Professional Support"
            description="Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit."
          />
        </swiper-slide>
        <swiper-slide>
          <Testimonial
            name="David Wilson"
            profession="Content Writer"
            image="https://picsum.photos/200/200?random=7.jpg"
            title="Exceptional Quality"
            description="Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur."
          />
        </swiper-slide>
        <swiper-slide>
          <Testimonial
            name="Sophia Martinez"
            profession="Web Developer"
            image="https://picsum.photos/200/200?random=8.jpg"
            title="Great Experience"
            description="Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit."
          />
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
