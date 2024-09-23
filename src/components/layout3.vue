<template>
    <section class="py-8">
      <div class="flex flex-wrap md:flex-nowrap space-x-0 md:space-x-4 p-4 space-y-4 md:space-y-0">
        <div
          v-for="(section, index) in sections"
          :key="index"
          :style="{ backgroundImage: `url(${section.bgImage})` }"
          class="w-full sm:w-1/2 md:w-1/3 h-64 bg-cover bg-center relative text-white p-6 rounded-lg overflow-hidden"
        >
          <div class="absolute inset-0 bg-black bg-opacity-40"></div>
          
          <div class="relative z-10 flex flex-col h-full justify-between">
            <span class="bg-teal-500 text-xs py-1 px-3 rounded-full inline-block self-start">
              {{ section.chip }}
            </span>
  
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
      bgImage: 'https://picsum.photos/1980/2400/?blur/?random=4',
      chip: 'New',
      heading: 'Explore Nature',
      description: 'Discover the beauty of the wild.',
    },
    {
      bgImage: 'https://picsum.photos/1980/2400/?blur/?random=5',
      chip: 'Trending',
      heading: 'City Life',
      description: 'Experience the urban vibe.',
    },
    {
      bgImage: 'https://picsum.photos/1980/2400/?blur/?random=6',
      chip: 'Popular',
      heading: 'Space Adventures',
      description: 'Journey to the stars.',
    }
  ]);
  </script>
  
  <style scoped>
  </style>
  