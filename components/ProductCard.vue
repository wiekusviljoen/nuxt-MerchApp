<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <NuxtLink :to="`/products/${product.id}`">
            <button class="my-4">View Details</button>
        </NuxtLink>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style  scoped>
.thumb {
    max-height: 120px;
    max-width: 70%;
    margin: 0 auto;
    border-radius: 5%;


}

.card {
    padding: 3px;
    border-radius: 10%;
    background-color: white
}

button {
    background-color: aqua;
    border-radius: 10px;
    padding: 4px;
}
</style>