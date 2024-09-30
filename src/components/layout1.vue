<template>
  <section>
    <div class="h-screen flex flex-wrap justify-center">
      <div
        v-for="(section, index) in sections"
        :key="index"
        :style="{ backgroundColor: section.bgColor }"
        class="w-full sm:w-1/2 md:w-1/4 text-white flex-col space-y-4 p-6 md:p-8 justify-center"
      >
        <div
          class="py-6 px-8 border-solid border border-white rounded-full inline-block mb-8"
        >
          <span class="text-xl font-bold">{{ index + 1 }}</span>
        </div>
        <div class="flex-col space-y-6">
          <h4>{{ section.heading }}</h4>
          <p class="font-thin">{{ section.description }}</p>
          <router-link class="font-thin underline">Read More</router-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const sections = ref([
  {
    heading: "This is the heading",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse, voluptatem.",
    bgColor: "#39399B",
  },
  {
    heading: "Another Heading",
    description: "Another description for this section.",
    bgColor: "#433FB5",
  },
  {
    heading: "Yet Another Heading",
    description: "Yet another description for this section.",
    bgColor: "#39399B",
  },
  {
    heading: "Yet Another Heading",
    description: "Yet another description for this section.",
    bgColor: "#433FB5",
  },
]);
</script>

<style scoped>
.bg-img{
  width: 100%;
  height: 100vh;
  background-image: url('../assets/framw.png');
  background-position: center;
  background-repeat: center;
  object-fit: cover;
}
</style>
