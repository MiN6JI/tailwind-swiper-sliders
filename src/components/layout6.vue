<template>
  <section class="py-8 flex flex-col justify-center items-center">
    <div class="w-full max-w-3xl flex flex-col justify-center items-center overflow-hidden rounded-md">
      <div class="w-full flex flex-col md:flex-row bg-cyan-950">
        <div class="w-full md:w-1/3 p-6 flex justify-center">
          <img class="profile-img" src="../assets/girl.jpg" alt="person">
        </div>
        <div class="w-full md:w-2/3 p-6 flex flex-col justify-center">
          <div class="text-white flex flex-col justify-center md:justify-start md:items-start items-center space-y-4">
            <p>Don't wait, call us today!</p>
            <h1 class="text-4xl">+91 46578 75678</h1>
          </div>
        </div>
      </div>
      <div class="w-full flex flex-col md:flex-row bg-gray-200 py-6">
        <div class="w-full md:w-1/3 p-4 flex flex-col justify-center items-center">
          <p class="text-center">Follow us on social media:</p>
          <div class="flex space-x-4 mt-2">
            <a href="#" class="bg-white p-2 rounded">
              <img src="../assets/facebook.png" alt="facebook" width="20">
            </a>
            <a href="#" class="bg-white p-2 rounded">
              <img src="../assets/instagram.png" alt="insta" width="20">
            </a>
            <a href="#" class="bg-white p-2 rounded">
              <img src="../assets/twitter.png" alt="twitter" width="20">
            </a>
          </div>
        </div>
        <div class="w-full md:w-2/3 py-4 px-4 md:px-8">
          <form class="flex flex-col space-y-4 mt-2">
            <input type="text" placeholder="Your Name" class="p-2 rounded border" required>
            <input type="email" placeholder="Your Email" class="p-2 rounded border" required>
            <textarea placeholder="Your Message" class="p-2 rounded border" rows="4" required></textarea>
            <button type="submit" class="bg-cyan-950 text-white p-2 rounded">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.profile-img {
  width: 100%;
  height: auto;
  max-width: 200px;
  border-radius: 10px;
}

@media (max-width: 768px) {
  .profile-img {
    max-width: 150px;
  }
}
</style>

