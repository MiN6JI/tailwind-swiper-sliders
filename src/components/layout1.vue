<template>
    <section>
        <div class="flex flex-row">
            <div
                v-for="(section, index) in sections"
                :key="index"
                :style="{ width: section.width }"
                :class="`bg-[${section.bgColor}] text-white flex-col space-y-4 p-16 justify-center`"
            >
                <div class="py-6 px-8 border-solid border border-white rounded-full inline-block mb-8">
                    <span class="text-xl font-bold">{{ index + 1 }}</span>
                </div>
                <div class="flex-col space-y-6">
                    <h4>{{ section.heading }}</h4>
                    <p class="font-thin text-caption">{{ section.description }}</p>
                    <router-link class="font-thin underline">Read More</router-link>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

const sections = ref([
    {
        heading: 'This is the heading',
        description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse, voluptatem.',
        bgColor: '#39399B',
        width: '33.33%' // User can adjust this value
    },
    {
        heading: 'Another Heading',
        description: 'Another description for this section.',
        bgColor: '#433FB5',
        width: '33.33%' // User can adjust this value
    },
    {
        heading: 'Yet Another Heading',
        description: 'Yet another description for this section.',
        bgColor: '#39399B',
        width: '33.33%' // User can adjust this value
    },
    {
        heading: 'Yet Another Heading',
        description: 'Yet another description for this section.',
        bgColor: '#433FB5',
        width: '33.33%' // User can adjust this value
    }
]);
</script>

<style scoped></style>
