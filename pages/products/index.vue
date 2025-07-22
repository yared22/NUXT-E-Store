<template>
  <div class="container mx-auto p-8">
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
      <div v-for="p in products" :key="p.id">
        <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink>
        </div>
    </div>
    </div>
</template>
<script setup>
import { NuxtLink } from '#components';

const {data:products} = await useFetch('https://fakestoreapi.com/products')

</script>
