<template>
  <div class="max-w-2xl mx-auto my-10 p-5 bg-gray-50 rounded-lg shadow-lg font-sans text-gray-700">
    <p>{{ product.title }}</p>
     <NuxtLink to="/" class="text-blue-500 no-underline font-semibold transition-colors duration-300 hover:text-blue-700 hover:underline">Home</NuxtLink>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri= "https://fakestoreapi.com/products/" + id;
const {data:product} = await useFetch(uri);
definePageMeta({
    layout: "products"
})
</script>


