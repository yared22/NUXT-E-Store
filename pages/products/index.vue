<template>
  <div class="container mx-auto p-8">
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
      <div v-for="p in products" :key="p.id">
        <ProductCard :product="p"/>
        </div>
    </div>
    </div>
</template>
<script setup>
import { NuxtLink } from '#components';
import ProductCard from '~/components/productCard.vue';

const {data:products} = await useFetch('https://fakestoreapi.com/products')

</script>
