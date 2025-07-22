<template>
    <div class="max-w-2xl mx-auto bg-white rounded-lg shadow-lg overflow-hidden">
        <div class="flex flex-col md:flex-row">
            <div class="md:w-1/3 p-6 flex justify-center items-center bg-gray-50">
                <img :src="product.image" alt="Product_image" class="h-48 w-48 object-contain" />
            </div>
            <div class="md:w-2/3 p-6">
                <h1 class="text-2xl font-bold text-gray-800 mb-4">{{ product.title }}</h1>
                <p class="text-gray-600 text-base mb-4 leading-relaxed">{{ product.description }}</p>
                <div class="space-y-2">
                    <p class="text-gray-700"><span class="font-semibold">Price:</span> ${{ product.price }}</p>
                    <p class="text-gray-700"><span class="font-semibold">Category:</span> {{ product.category }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>