<template>
  <div class="flex flex-col md:flex-row space-y-4 md:space-y-0">
    <div class="w-full md:w-1/5 flex justify-center items-center">
      <img class="w-full h-full object-cover" :src="image" alt="random" />
    </div>

    <div class="w-full md:w-4/5 text-center md:text-left py-4 px-6">
      <div class="flex flex-row justify-between py-2">
        <div>
          <h4 class="text-lg md:text-xl font-medium text-yellow-500 py-2 capitalize">{{ title }}</h4>
        </div>
        <div class="flex flex-col justify-center">
          <p class="text-gray-500">{{ day }}</p>
        </div>
      </div>
      <h4 class="text-lg md:text-xl font-bold text-gray-800 capitalize">{{ textTitle }}</h4>
      <p class="text-sm md:text-base text-gray-500">{{ description }}</p>

      <div
        class="flex flex-col md:flex-row items-center md:items-start py-4 space-y-4 md:space-y-0 md:space-x-6"
      >
        <div class="flex justify-center items-center">
          <img
            class="w-10 h-10 md:w-8 md:h-8 lg:w-10 lg:h-10 rounded-full"
            :src="profileImg"
            alt="random-img"
          />
        </div>
        <div class="text-center md:text-left">
          <h4 class="text-base md:text-lg font-bold text-gray-800">{{ profileName }}</h4>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  image: String,
  title: String,
  day: String,
  textTitle: String,
  description: String,
  profileImg: String,
  profileName: String,
});
</script>
