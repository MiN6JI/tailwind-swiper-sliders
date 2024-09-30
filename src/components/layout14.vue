<template>
  <section class="bg-img flex flex-col justify-center items-center">
    <div
      class="card shadow-2xl bg-white w-3/5 rounded-lg flex flex-col justify-center items-center overflow-hidden"
    >
      <div class="bg-[#182F35] p-6 text-white relative">
        <div class="static flex flex-row w-full">
          <div class="w-1/3 relative">
            <img
              class="profile static md:relative md:top-12 rounded-md"
              src="../assets/girl.jpg"
              alt="girl"
            />
          </div>
          <div class="w-2/3 py-4 px-10 flex flex-col space-y-4 justify-center">
            <div class="text-white">Don't wait! Call us Today</div>
            <div class="text-3xl text-teal-400">+91 897967 34253</div>
          </div>
        </div>
      </div>
      <div class="flex flex-row w-full py-6 px-10">
        <div class="w-1/3 p-4 flex flex-col justify-center items-start">
          <div>or write an e-mail</div>
          <div class="text-xl font-medium">xyz@gmail.com</div>
          <div class="py-4">
            <div class="flex flex-row space-x-2">
              <div class="p-2 bg-gray-300">
                <i class="fa-brands fa-facebook"></i>
              </div>
              <div class="p-2 bg-gray-300">
                <i class="fa-brands fa-instagram"></i>
              </div>
              <div class="p-2 bg-gray-300">
                <i class="fa-brands fa-twitter"></i>
              </div>
              <div class="p-2 bg-gray-300">
                <i class="fa-brands fa-youtube"></i>
              </div>
            </div>
          </div>
        </div>
        <div class="w-2/3 p-4">
            <form @submit.prevent="handleSubmit">
            <div class="flex flex-col space-y-2">
              <div>
                <input
                  v-model="form.name"
                  type="text"
                  id="name"
                  class="text-sm block w-full border-b border-gray-300 p-1"
                  placeholder="Name"
                  required
                />
              </div>
              <div>
                <input
                  v-model="form.email"
                  type="email"
                  id="email"
                  class="text-sm block w-full border-b border-gray-300 p-1"
                  placeholder="Email"
                  required
                />
              </div>
              <div>
                <input
                  v-model="form.subject"
                  type="text"
                  id="subject"
                  class="text-sm block w-full border-b border-gray-300 p-1"
                  placeholder="Subject"
                  required
                />
              </div>
              <div>
                <textarea
                  v-model="form.message"
                  id="message"
                  rows="2"
                  class="text-sm block w-full border-b border-gray-300 p-1"
                  placeholder="Message"
                  required
                ></textarea>
              </div>
              <button
                type="submit"
                class="mt-4 bg-teal-400 text-white py-1 px-4 rounded-full hover:bg-teal-500 transition duration-200"
              >
                Send Message
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const form = ref({
  name: '',
  email: '',
  subject: '',
  message: '',
});

const handleSubmit = () => {
  // Handle form submission logic here
  console.log('Form submitted:', form.value);
  
  // Clear the form after submission
  form.value = {
    name: '',
    email: '',
    subject: '',
    message: '',
  };
};
</script>
<style scoped>
.bg-img {
  width: 100%;
  height: 100vh;
  background-image: url("../assets/framw.png");
  background-position: center;
  background-repeat: no-repeat;
  object-fit: cover;
}

.profile {
  /* width: 100%; */
  /* height: 200px; */
}
</style>
