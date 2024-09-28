<template>
  <div class="card">
    <div class="w-full flex flex-col space-y-6">
      <img src="../assets/girl.jpg" alt="profile" />
      <div class="flex flex-col justify-center items-center space-y-4 p-4">
        <h1 class="text-2xl font-bold">John Doe</h1>
        <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque, dolores.</p>
        <div class="flex space-x-6 py-8">
            <i class="fa-brands fa-facebook fa-xl text-black"></i>
            <i class="fa-brands fa-instagram fa-xl text-black"></i>
            <i class="fa-brands fa-twitter fa-xl text-black"></i>
        </div>
      </div>
    </div>

    <div class="card-body flex flex-col justify-center items-center space-y-6">
      <h1 class="text-3xl font-bold capitalize">John Doe</h1>
      <p class="font-light capitalize">Software Engineer</p>

      <div class="flex space-x-4">
        <div class="py-1 px-2 rounded-full bg-white">
            <i class="fa-brands fa-facebook fa-sm text-gray-400"></i>
        </div>
        <div class="py-1 px-2 rounded-full bg-white">
            <i class="fa-brands fa-instagram fa-md text-gray-400"></i>
        </div>
        <div class="py-1 px-2 rounded-full bg-white">
            <i class="fa-brands fa-twitter fa-md text-gray-400"></i>
        </div>
    </div>
    <router-link class="text-center border rounded-full border-white py-2 px-6" >More Details</router-link>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.card {
  overflow: hidden;
  position: relative;
}

.card-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 15px;
}

.card-body {
  width: 100%;
  height: 100%;
  top: 0;
  right: -100%;
  position: absolute;
  background: linear-gradient(90deg, rgba(57, 136, 231, 0.7) 0%, rgba(219, 48, 238, 0.7) 50%);
  backdrop-filter: blur(5px);
  color: #fff;
  padding: 30px;
  transition: 2s;
}

.card:hover .card-body {
  right: 0;
}

</style>
