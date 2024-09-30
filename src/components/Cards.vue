<template>
  <div class="w-full h-full p-2 flex flex-col justify-start items-start space-y-4">
    <div class="w-full rounded-md overflow-hidden">
      <img class="blog-img" :src="blogImg" alt="blog-img">
    </div>
    <div class="px-4">
      <div class="block py-2 px-6 rounded-lg text-sm capitalize bg-indigo-100 text-indigo-600 font-bold">
      {{ chip }}
    </div>
    </div>
    <div class="w-full px-4 pb-6 text-left flex flex-col space-y-4">
      <div class="text-xl capitalise font-bold text-gray-700">{{ title }}</div>
      <p class="text-gray-500 text-sm">{{ description }}</p>
      <div class="flex flex-row space-x-4 py-2">
        <img class="rounded-full" :src="profile" alt="profile-img" width="40px" height="40" >
        <div>
          <div class="text-sm font-bold">{{ name }}</div>
          <div class="text-xs text-gray-500">{{ day }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import Profile from './profile.vue';

defineProps({
  blogImg: String,
  chip: String,
  title: String,
  description: String,
  profile: String,
  name: String,
  day: String
});
</script>

<style scoped>
.blog-img{
  width: 100%;
  height: 250px;
  object-fit: cover;
}

/* .chip{
  max-width: 150px;
} */
</style>
