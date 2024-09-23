<template>
    <section
      class="bg-img h-screen bg-cover bg-center text-white p-10 flex flex-col justify-between"
    >
      <!-- Heading -->
      <h1 class="text-4xl md:text-6xl font-bold text-center mb-8">Biography</h1>
  
      <!-- Responsive 3-column layout -->
      <div class="w-full max-w-6xl grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8 mx-auto">
        <!-- First Column -->
        <div class="bg-gray-800 bg-opacity-75 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Early Life</h3>
          <p class="text-sm">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae ante erat.
          </p>
        </div>
  
        <!-- Second Column -->
        <div class="bg-gray-800 bg-opacity-75 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Career</h3>
          <p class="text-sm">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae ante erat.
          </p>
        </div>
  
        <!-- Third Column -->
        <div class="bg-gray-800 bg-opacity-75 p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-4">Achievements</h3>
          <p class="text-sm">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae ante erat.
          </p>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  .bg-img {
    background-image: url('https://picsum.photos/1980/1280?random=9/?grayscale');
    background-position: center;
    background-repeat: no-repeat;
  }
  
  /* Ensure proper height on smaller screens */
  @media (max-width: 768px) {
    .h-screen {
      height: auto;
    }
  }
  </style>
  