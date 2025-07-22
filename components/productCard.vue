<template>
  <div class="card text-center">
    <NuxtLink :to="`/products/${product.id}`">
      <img :src="product.image" alt="Product_image" class="thumb" />
      <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
    </NuxtLink>
  </div>
</template>

<script setup>
import { NuxtLink } from "#components";

const { product } = defineProps(["product"]);
</script>

<style scoped>
.thumb {
  max-height: 120px;
  max-width: 70px;
  margin: 0 auto;
}
</style>
