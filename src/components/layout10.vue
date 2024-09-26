<template>
  <div class="w-full bg-white shadow-lg rounded-lg flex">
    <div class="w-3/5 p-4 flex flex-col justify-between bg-blue-700">
      <div class="w-full flex flex-row justify-center ">
        <div class="w-1/3 flex flex-col justify-center text-white">
          <h2 class="text-2xl font-bold mb-4 ">Your Personal Car Rental</h2>
          <p class="text-gray-100 mb-6">
            Book your next adventure with our reliable car rental service.
          </p>
        </div>
        <div class="w-2/3 p-4">
          <form @submit.prevent="handleSubmit">
            <div class="mb-4">
              <input type="text" id="name" v-model="formData.name" placeholder="Name"
                class="mt-1 block w-full border border-gray-300 rounded-md p-2" required />
            </div>
            <div class="mb-4">
              <input type="email" id="email" v-model="formData.email" placeholder="Email"
                class="mt-1 block w-full border border-gray-300 rounded-md p-2" required />
            </div>
            <div class="mb-4">
              <textarea id="message" v-model="formData.message" rows="3" placeholder="Message"
                class="mt-1 block w-full border border-gray-300 rounded-md p-2"></textarea>
            </div>
            <button type="submit" class="w-full text-white bg-teal-5  00 py-2 rounded-md hover:bg-blue-700">
              Book Now
            </button>
          </form>
        </div>
      </div>
    </div>
    <div class="w-2/5">
      <img class="w-full h-80" src="../assets/girl.jpg" alt="Car Rental Image" style="object-fit: cover;" />
    </div>
  </div>
</template>
<script setup>
import { ref } from 'vue';

const formData = ref({
  name: '',
  email: '',
  message: '',
});

const handleSubmit = () => {
  console.log('Form submitted:', formData.value);
  // Reset form fields if needed
  formData.value = { name: '', email: '', message: '' };
};
</script>
