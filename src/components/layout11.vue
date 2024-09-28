<template>
    <section class="py-8 flex justify-center items-center">
        <div :class="getCardClasses()" class="rounded-lg w-full md:w-2/3 lg:w-1/2 py-4 px-6 md:px-8 text-white flex flex-col justify-between">
            <div>
                <h3 class="text-2xl font-bold py-3">All your credentials in one place</h3>
                <p v-if="!buttonClicked">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, doloribus quasi asperiores rerum architecto cum adipisci mollitia ipsam eaque beatae!</p>
                <p v-if="buttonClicked" class="appear">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nam obcaecati ullam deserunt rerum natus culpa eaque eligendi? Quod tenetur expedita deserunt officiis, rerum ad veniam placeat vitae! Facere odit illum eos excepturi in mollitia? Sed laboriosam nobis harum, quae aperiam reiciendis alias, aspernatur mollitia expedita quis corrupti, quas natus nemo provident odio. Cum neque accusamus doloremque harum nisi! Odio esse sint quidem? Explicabo, facilis nostrum in amet maiores asperiores qui labore? Odit quae aspernatur, debitis accusamus tenetur possimus nam repellat mollitia officiis magni soluta numquam? Ab fugiat architecto dolorem mollitia ipsa, harum temporibus praesentium maxime quidem nesciunt esse quod reprehenderit.</p>
                <img v-if="!buttonClicked" src="../assets/dashboard-1.png" alt="Image" class="my-12 rounded-lg w-full h-auto">
            </div>
            <div>
                <div class="p-2">
                    <img 
                        src="../assets/plus.png" 
                        alt="button" 
                        width="50px" 
                        @click="toggleContent" 
                        :class="{ 'rotate-45': buttonClicked }"
                    >
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

const buttonClicked = ref(false);

function toggleContent() {
    buttonClicked.value = !buttonClicked.value;
}

function getCardClasses() {
    return ['card', { 'bg-blue': buttonClicked.value }];
}
</script>

<style scoped>
.card {
    height: 550px;
    max-height: 100vh;
    background: linear-gradient(90deg, rgba(26,103,200,1) 0%, rgba(179,53,155,1) 35%, rgba(255,68,0,1) 100%);
    transition: background 0.3s ease;
}

.bg-blue {
    background: rgb(78, 78, 230);
}

.rotate-45 {
    transition: transform 0.3s ease;
    transform: rotate(45deg);
}
</style>
