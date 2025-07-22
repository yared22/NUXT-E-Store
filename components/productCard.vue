<template>
  <div class="bg-white rounded-lg shadow-md p-4 border border-gray-200 text-center
   hover:shadow-lg transition-shadow duration-300">
    <NuxtLink :to="`/products/${product.id}`" class="block">
      <img :src="product.image" alt="Product_image" class="h-30 w-18 mx-auto mb-3 object-contain" />
      <p class="font-bold text-gray-700 
      text-sm truncate hover:text-blue-600
       transition-colors duration-200">
       {{ product.title }}</p>
    </NuxtLink>
  </div>
</template>

<script setup>
import { NuxtLink } from "#components";

const { product } = defineProps(["product"]);
</script>


