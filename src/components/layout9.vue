<template>
  <section class="py-8">
    <div class="w-full max-w-3xl mx-auto bg-white shadow-lg rounded-lg overflow-hidden flex flex-col md:flex-row">
      <img
        class="w-full md:w-1/2 object-cover"
        src="../assets/girl.jpg"
        alt="Item image"
      />
      <div class="w-full md:w-1/2 px-4 py-10 flex flex-col justify-center">
        <div>
          <h2 class="text-xl font-bold">{{ item.name }}</h2>
          <p class="text-gray-600">{{ item.experience }}</p>
          <p class="mt-2 text-gray-700">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque
            sit amet accumsan arcu.
          </p>
        </div>
        <div class="flex justify-start space-x-4 my-6">
          <img src="../assets/award.png" alt="medal" width="50px">
          <img src="../assets/award.png" alt="medal" width="50px">
          <img src="../assets/award.png" alt="medal" width="50px">
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
      },
    };
  },
};
</script>

<style scoped>
</style>
