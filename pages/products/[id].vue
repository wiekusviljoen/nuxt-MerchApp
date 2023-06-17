<template>
    <div>
        <p>Products details for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem repudiandae dignissimos neque ad fugit
            omnis, rem nihil non at ipsa consequatur laboriosam ipsum explicabo facere. A ex explicabo eaque eos.</p>
    </div>
</template>

<script setup>
const { id } = useRoute().params()
definePageMeta({ layout: "products" })
</script>

<style scoped></style>