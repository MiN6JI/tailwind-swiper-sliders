<template>
    <div class="flex flex-col md:flex-row space-y-4 md:space-y-0">
      <!-- Image Section -->
      <div class="w-full md:w-1/5 flex justify-center items-center">
        <img
          class="w-full md:w-auto h-full"
          src="https://picsum.photos/seed/picsum/300/200?random=2.jpg"
          alt="random-img"
        />
      </div>
      
      <!-- Text Section -->
      <div class="w-full md:w-4/5 text-center md:text-left p-4">
        <h4 class="text-lg md:text-xl font-medium text-yellow-500 py-2">Good News</h4>
        <h4 class="text-lg md:text-xl font-bold text-gray-800">Our Four-legged Warriors</h4>
        <p class="text-sm md:text-base text-gray-500">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque ut nam odit tenetur, laborum voluptatum sunt ea voluptate dolores culpa?
        </p>
  
        <!-- Inner Section -->
        <div class="flex flex-col md:flex-row items-center md:items-start py-4 space-y-4 md:space-y-0 md:space-x-6">
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
            <h4 class="text-base md:text-lg font-bold text-gray-800">John Doe</h4>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup></script>
  