<template>
  <section class="py-8">
    <div class="w-full max-w-3xl mx-auto bg-white shadow-lg rounded-lg overflow-hidden flex flex-col md:flex-row">
      <img
        class="w-full md:w-1/2 object-cover"
        :src="item.image"
        alt="Item image"
      />
      <div class="w-full md:w-1/2 p-4 flex flex-col justify-center">
        <div>
          <h2 class="text-xl font-bold">{{ item.name }}</h2>
          <p class="text-gray-600">{{ item.experience }}</p>
          <p class="mt-2 text-gray-700">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque
            sit amet accumsan arcu.
          </p>
        </div>
        <div class="flex justify-center space-x-4 mt-4">
          <img
            v-for="(logo, index) in item.logos"
            :key="index"
            :src="logo"
            class="w-12 h-auto"
            alt="Logo"
          />
        </div>
        <p class="mt-2 text-gray-700">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque
          sit amet accumsan arcu.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      item: {
        image: 'https://via.placeholder.com/400',
        name: 'John Doe',
        experience: '5 years of experience in web development',
        logos: [
          'https://via.placeholder.com/50',
          'https://via.placeholder.com/50',
          'https://via.placeholder.com/50',
        ],
      },
    };
  },
};
</script>

<style scoped>
</style>
