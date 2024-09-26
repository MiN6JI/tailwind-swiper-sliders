<template>
  <section class="md:h-screen flex flex-row justify-center items-center">
    <div class="flex flex-wrap md:flex-nowrap space-x-0 md:space-x-4 p-4 space-y-4 md:space-y-0">
        <div
          v-for="(section, index) in sections"
          :key="index"
          :style="{ backgroundImage: `url(${section.bgImage})` }"
          class="w-full sm:w-1/2 md:w-1/3 h-64 md:h-80 bg-cover bg-center relative text-white p-6 rounded-lg overflow-hidden"
        >
          <div class="absolute inset-0 bg-black bg-opacity-40"></div>
          
          <div class="relative z-10 flex flex-col h-full justify-end">
            
            <div class="mt-4">
              <h3 class="text-xl font-bold">{{ section.heading }}</h3>
              <p class="mt-2 text-sm">{{ section.description }}</p>
            </div>
          </div>
        </div>
      </div>
      </section>
</template>

<script setup>
import { ref } from 'vue';

const sections = ref([
  {
    bgImage: 'https://picsum.photos/1980/2400/?blur/?random=14',
    chip: 'New',
    heading: 'Explore Nature',
    description: 'Discover the beauty of the wild.',
  },
  {
    bgImage: 'https://picsum.photos/1980/2400/?blur/?random=15',
    chip: 'Trending',
    heading: 'City Life',
    description: 'Experience the urban vibe.',
  },
  {
    bgImage: 'https://picsum.photos/1980/2400/?blur/?random=16',
    chip: 'Popular',
    heading: 'Space Adventures',
    description: 'Journey to the stars.',
  },
  {
    bgImage: 'https://picsum.photos/1980/2400/?blur/?random=17',
    chip: 'Popular',
    heading: 'Explore Kitchen',
    description: 'Food for Life',
  }
]);
</script>

<style scoped>

section{
  background-image: url('../assets/john-towner-JgOeRuGD_Y4-unsplash.jpg');
  background-position: center;
  background-repeat: no-repeat;
  object-fit: cover;
}
</style>