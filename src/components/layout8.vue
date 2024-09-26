<template>
  <div class="grid grid-cols-2 grid-rows-2 gap-4 p-4">
    <div class="col-span-2 row-span-1 bg-cover bg-center relative h-64" :style="{ backgroundImage: `url('${item1.image}')` }">
      <div class="absolute inset-0 bg-black bg-opacity-30 flex flex-col justify-center items-start p-4">
        <h2 class="text-white text-xl font-bold">{{ item1.title }}</h2>
        <p class="text-white">{{ item1.subtext }}</p>
      </div>
    </div>
    <div class="col-span-1 row-span-1 bg-cover bg-center relative h-64" :style="{ backgroundImage: `url('${item2.image}')` }">
      <div class="absolute inset-0 bg-black bg-opacity-30 flex flex-col justify-center items-start p-4">
        <h2 class="text-white text-xl font-bold">{{ item2.title }}</h2>
        <p class="text-white">{{ item2.subtext }}</p>
      </div>
    </div>
    <div class="col-span-1 row-span-1 bg-cover bg-center relative h-64" :style="{ backgroundImage: `url('${item3.image}')` }">
      <div class="absolute inset-0 bg-black bg-opacity-30 flex flex-col justify-center items-start p-4">
        <h2 class="text-white text-xl font-bold">{{ item3.title }}</h2>
        <p class="text-white">{{ item3.subtext }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      item1: {
        image: 'https://via.placeholder.com/400',
        title: 'Item 1',
        subtext: 'Description for item 1',
      },
      item2: {
        image: 'https://via.placeholder.com/400',
        title: 'Item 2',
        subtext: 'Description for item 2',
      },
      item3: {
        image: 'https://via.placeholder.com/400',
        title: 'Item 3',
        subtext: 'Description for item 3',
      },
    };
  },
};
</script>
