<template>
    <div class="img-card px-4 py-6 flex flex-col justify-end items-center space-y-4" :style="{ backgroundImage: `url(${image})` }">
        <h1 class="text-2xl font-bold text-white">{{ heading }}</h1>
        <p class="text-white">{{ paragraph }}</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    heading: {
        type: String,
        required: true,
    },
    paragraph: {
        type: String,
        required: true,
    },
    image: {
        type: String,
        required: true,
    },
});
</script>

<style scoped>
.img-card {
    width: 100%;
    height: 100%;
    background-repeat: no-repeat;
    background-size: cover; /* Ensures the image covers the entire div */
    background-position: center;
}
</style>
