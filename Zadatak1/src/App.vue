<script setup>
</script>

<template>
   <!-- Glavni wrapper (pozadina + centriranje) -->
  <div ref="dark" class="min-h-screen bg-gray-200 dark:bg-gray-900 flex items-center justify-center p-6 relative">

      <!-- Gumb za temu -->
      <div class="absolute top-4 right-4 md:top-6 md:right-6">
      <button
      @click="$refs.dark.classList.toggle('dark');"
      class="text-xs md:text-sm px-2 md:px-3 py-1 bg-gray-100 dark:bg-gray-800 dark:text-gray-300 rounded-md">
      Promijeni temu
      </button>
      </div>

      <!-- Glavna kartica  -->
    <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-lg p-8 w-full max-w-5xl">

      <!-- Naslov -->
      <h1 class="text-2xl text-center font-semibold dark:text-gray-300">
        Pozdrav, ja sam 
        <span class="text-orange-500 font-bold">Anja Svećarovski</span>
      </h1>

      <hr class="my-4 border-gray-400 dark:border-gray-600">

      <!-- Podnaslov -->
      <h2 class="text-lg text-gray-700 dark:text-gray-300 mb-6">
        Moji omiljeni filmovi
      </h2>

      <!-- Filmovi -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">

        <!-- Film 1 -->
        <div class="text-center">
          <img 
            src="/HMC.jpg" 
            class="rounded-lg shadow-md mb-3"
          >
          <p class="font-semibold dark:text-gray-200">Howl's Moving Castle</p>
        </div>

        <!-- Film 2 -->
        <div class="text-center">
          <img 
            src="/PM.jpg" 
            class="rounded-lg shadow-md mb-3"
          >
          <p class="font-semibold dark:text-gray-200">Princess Mononoke</p>
        </div>

        <!-- Film 3 -->
        <div class="text-center">
          <img 
            src="/YN.jpg" 
            class="rounded-lg shadow-md mb-3"
          >
          <p class="font-semibold dark:text-gray-200">Your Name</p>
        </div>

      </div>

    </div>
  </div>
</template> 

<style scoped>
</style>
