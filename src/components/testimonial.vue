<template>
  <div class="flex flex-col space-y-6 p-4 md:p-6">
    <div class="flex flex-col md:flex-row space-y-4 md:space-y-0">
      <div class="w-full md:w-1/5 flex sm:justify-center items-center">
        <img
          class="w-10 h-10 md:w-6 md:h-6 lg:w-10 lg:h-10 rounded-full"
          :src="image"
          alt="profile"
        />
      </div>
      <div class="w-full md:w-4/5 text-center md:text-left">
        <h4 class="text-xl md:text-lg font-bold text-gray-800">{{ name }}</h4>
        <p class="text-sm text-gray-500">{{ profession }}</p>
      </div>
    </div>
    <div>
      <h6 class="text-lg font-bold text-gray-800 text-left">{{ title }}</h6>
      <p class="text-sm text-gray-500 text-left">{{ description }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  profession: String,
  image: String,
  title: String,
  description: String
});
</script>