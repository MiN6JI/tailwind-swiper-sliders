<template>
  <section class="p-4">
    <div class="w-full flex flex-row gap-4">
      <div class="1/5">
        <ImgCard />
      </div>
      <div class="w-1/3 img-2"></div>
      <div class="w-1/3 img-3"></div>
    </div>
  </section>
</template>
<script setup>
import ImgCard from './ImageCard.vue'

</script>
<style scoped>
.img-1 {
  background-image: url("https://picsum.photos/200/300?random=1");
  object-fit: cover;
  background-repeat: no-repeat;
}
</style>
