<template>
  <section class="bg-gray-50 py-10">
    <div class="flex flex-col space-y-4">
      <div class="flex flex-col md:flex-row">
        <div class="flex-1">
          <div class="p-4">
            <img src="../assets/logo.svg" alt="logo" width="180px" />
            <p class="text-gray-500 py-4 text-sm">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Qui
              facilis repudiandae provident aperiam. Voluptates, fugit rem
              architecto quos!
            </p>
            <div class="flex flex-row space-x-6 py-6">
              <i class="fa-brands fa-facebook text-teal-400 fa-lg"></i>
              <i class="fa-brands fa-instagram text-teal-400 fa-lg"></i>
              <i class="fa-brands fa-twitter text-teal-400 fa-lg"></i>
              <i class="fa-brands fa-github text-teal-400 fa-lg"></i>
            </div>
          </div>
        </div>
        <div class="flex-1 flex flex-col md:flex-row justify-around items-start">
          <div class="flex flex-col space-y-2">
            <div class="font-bold text-lg py-4">
              About Us
            </div>
          <router-link class="text-md text-gray-500 font-medium">Home</router-link>
          <router-link class="text-md text-gray-500 font-medium">About</router-link>
          <router-link class="text-md text-gray-500 font-medium">History</router-link>
          <router-link class="text-md text-gray-500 font-medium">Services</router-link>

        </div>
        <div class="flex flex-col space-y-2">
            <div class="font-bold text-lg py-4">
              Our Services
            </div>
          <router-link class="text-md text-gray-500 font-medium">Home</router-link>
          <router-link class="text-md text-gray-500 font-medium">About</router-link>
          <router-link class="text-md text-gray-500 font-medium">History</router-link>
          <router-link class="text-md text-gray-500 font-medium">Services</router-link>

        </div>
        </div>
        <div class="flex-1 flex flex-col md:flex-row justify-around items-start">
          <div class="flex-1 flex justify-center">
            <div class="flex flex-col space-y-2">
            <div class="font-bold text-lg py-4">
              Helpful Links
            </div>
          <router-link class="text-md text-gray-500 font-medium">FAQ</router-link>
          <router-link class="text-md text-gray-500 font-medium">Support</router-link>
          <router-link class="text-md text-gray-500 font-medium">Live Chat</router-link>
        </div>
          </div>
        <div class=" flex-1 flex flex-col space-y-2">
          <div class="font-bold text-lg py-4">
              Contacts
            </div>
          <div class="flex flex-row justify-center items-center space-x-2">
            <i class="w-1/6 fa-regular fa-envelope text-gray-500 fa-lg"></i>
            <div class="w-5/6 text-md text-gray-600">xyz@gmail.com</div>
          </div>
          <div class="flex flex-row justify-center items-center space-x-2">
            <i class="w-1/6 fa-solid fa-phone text-gray-500 fa-lg"></i>
            <div class="w-5/6 text-md text-gray-600">+91 99767 86355</div>
          </div>
          <div class="flex flex-row justify-center items-center space-x-2">
            <i class="w-1/6 fa-solid fa-location-dot text-gray-500 fa-lg"></i>
            <div class="w-5/6 text-md text-gray-600">
              Maplewood Drive
              <br>
              Springfield
              <br>
              United States
            </div>
          </div>
        </div>
        </div>
      </div>
      <hr /> 
      <div class="flex flex-col md:flex-row px-4 py-2">
        <div class="flex-1 text-gray-600">© Kefitup</div>
        <div class="flex-1 flex justify-end space-x-4">
          <div>All rights reserved.</div>
          <router-link class="underline underline-offset-2 text-teal-400">Terms & Conditions</router-link>
          <router-link class="underline underline-offset-2 text-teal-400">Privacy Policy</router-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style scoped></style>
