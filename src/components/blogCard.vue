<template>
    <div class="w-full flex flex-col md:flex-row">
      <div class="md:w-2/5">
        <div class="border-r flex flex-col md:flex-row justify-around items-center md:items-stretch p-4">
          <img :src="imageUrl" alt="blog image" class="blog-img rounded-md">
          <div class="flex flex-col justify-center items-center mt-4 md:mt-0">
            <h1 class="text-4xl font-extrabold">{{ day }}</h1>
            <p class="font-medium text-xl text-gray-600">{{ month }}</p>
          </div>
        </div>
      </div>
      <div class="md:w-3/5 py-4 px-4 md:px-8 flex flex-col md:flex-row space-x-4 justify-center items-center">
        <div class="text-2xl font-medium text-center md:text-left">{{ description }}</div>
        <router-link :to="link" class="py-4 md:py-0">
          <img src="../assets/next.png" alt="next" class="w-8 md:w-16">
        </router-link>
      </div>
    </div>
  </template>
  

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    day: {
        type: String,
        required: true,
    },
    month: {
        type: String,
        required: true,
    },
    description: {
        type: String,
        required: true,
    },
    imageUrl: {
        type: String,
        required: true,
    },
    link: {
        type: String,
        default: '#',
    },
});
</script>

<style scoped>
.blog-img {
    width: 350px;
    height: 200px;
    object-fit: cover;
}
</style>
