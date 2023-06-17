<template>
    <div class="background">
        <div class="card ">
            <div class="grid grid-cols-2 ">
                <div class="p-7 ml-10">
                    <img :src="product.image" alt="product img" class=",x-auto my-7">
                </div>
                <div class="p-7">
                    <h2 class="text-4xl my-7">{{ product.title }}</h2>
                    <p class="text-xl my-7">Price - ${{ product.price }}</p>
                    <h3 class="font-bold border-b-2 pb-2">Product Description:</h3>
                    <p class="mb-7">{{ product.description }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style  scoped>
.background {
    background-color: white;
    border-radius: 15px;
}

img {
    border-radius: 15px;
    max-width: 300px;


}
</style>