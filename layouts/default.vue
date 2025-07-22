<template>
  <a href="/" class="text-3xl font-bold text-gray-800">NUXTPRO</a>
  <div class="max-w-4xl mx-auto p-5 font-sans text-gray-800">
    <header>
      <nav class="bg-blue-500 px-5 py-2.5 rounded-lg mb-8 flex items-center font-semibold">
        <NuxtLink to="/" class="text-black no-underline mx-2.5 transition-colors duration-300 hover:text-blue-200 hover:underline" active-class="!text-orange-400 !font-bold !underline">Home</NuxtLink>
        <span class="text-white mx-1">|</span>
        <NuxtLink to="/about" class="text-black no-underline mx-2.5 transition-colors duration-300 hover:text-blue-200 hover:underline" active-class="!text-orange-400 !font-bold !underline">About</NuxtLink>
        <span class="text-white mx-1">|</span>
        <NuxtLink to="/products" class="text-black no-underline mx-2.5 transition-colors duration-300 hover:text-blue-200 hover:underline" active-class="!text-orange-400 !font-bold !underline">Products</NuxtLink>
      </nav>
    </header>
    <main class="bg-gray-50 p-8 rounded-lg shadow-lg min-h-96">
      <NuxtPage />
    </main>
  </div>
  <footer class="bg-gray-800 text-gray-300 p-5 text-center mt-8 font-sans text-sm">
    <p>&copy; {{ new Date().getFullYear() }} MyApp. All rights reserved.</p>
    <p class="text-xs text-gray-400 mt-1">Building dreams with every line of code.</p>
  </footer>
</template>

<script setup>
</script>
<style scoped>
*{
  background-color:antiquewhite;
}
</style>




