<template>
    <div class="w-full flex flex-row">
        <div class="w-2/5">
            <div class="border-r flex flex-row justify-around items-stretch">
                <img :src="imageUrl" alt="blog image" class="blog-img rounded-md">
                <div class="flex flex-col justify-center items-center">
                    <h1 class="text-4xl font-extrabold">{{ day }}</h1>
                    <p class="font-medium text-xl text-gray-600">{{ month }}</p>
                </div>
            </div>
        </div>
        <div class="w-3/5 py-4 px-8 flex flex-row space-x-4 justify-center items-center">
            <div class="text-2xl font-medium">{{ description }}</div>
            <router-link :to="link">
                <img src="../assets/next.png" alt="next" width="50">
            </router-link>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    day: {
        type: String,
        required: true,
    },
    month: {
        type: String,
        required: true,
    },
    description: {
        type: String,
        required: true,
    },
    imageUrl: {
        type: String,
        required: true,
    },
    link: {
        type: String,
        default: '#',
    },
});
</script>

<style scoped>
.blog-img {
    width: 350px;
    height: 200px;
    object-fit: cover;
}
</style>
