<template>
  <div class="p-2">
    <div>
      <img
        src="https://picsum.photos/seed/picsum/1200/1200?random=2.jpg"
        alt="placeholder-img"
        width="100%"
        height="200px"
      />
    </div>
    <div class="w-full text-center md:text-left p-4">
      <h4 class="py-2 text-lg md:text-xl font-bold text-gray-800 capitalize">
        A digital Marketing Stats We have seen this week
      </h4>
      <p class="text-sm md:text-base text-gray-500">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Harum
        praesentium eius officiis, voluptate cum, ut atque beatae sunt, odio
        neque rerum soluta? Incidunt nostrum, facilis voluptatibus doloribus vel
        officiis possimus.
      </p>

      <!-- Inner Section -->
      <div
        class="flex flex-col md:flex-row items-center md:items-start py-4 space-y-4 md:space-y-0 md:space-x-6"
      >
        <!-- Profile Image Section -->
        <div class="flex justify-center items-center">
          <img
            class="w-10 h-10 md:w-8 md:h-8 lg:w-10 lg:h-10 rounded-full"
            src="https://picsum.photos/seed/picsum/200/200?random=2.jpg"
            alt="random-img"
          />
        </div>

        <!-- Profile Text Section -->
        <div class="text-center md:text-left">
          <h4 class="text-base md:text-lg font-bold text-gray-500">John Doe</h4>
          <p class="text-gray-500 text-sm">22 Jan 2024, 15min</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
img{
    border-radius: 10px;
}
</style>
