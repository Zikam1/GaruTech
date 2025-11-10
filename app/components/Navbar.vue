<template>
  <nav class="bg-white shadow-md w-full z-50">
    <div class="container mx-auto px-6 py-4 flex justify-between items-center">
     
      <!-- Logo -->
      <NuxtLink to="/" class="flex items-center">
        <img src="/assest/kt2.png" alt="Garu-Logo"
          class="h-32 w-auto object-contain md:h-20 lg:h-24 transition-transform duration-300 hover:scale-105" />
      </NuxtLink>

      <!-- Phone Numbers (Center) -->
      <div class="hidden md:flex flex-col text-center space-y-1">
        <div class="flex items-center justify-center space-x-4 text-sm font-semibold text-gray-700">
          <a href="https://wa.me/2348023190606" target="_blank" class="hover:text-green-600 hover:underline">
            08023190606
          </a>
          <span>|</span>
          <a href="https://wa.me/2347084440011" target="_blank" class="hover:text-green-600 hover:underline">
            07084440011
          </a>
          <span>|</span>
          <a href="https://wa.me/2348037153017" target="_blank" class="hover:text-green-600 hover:underline">
            08037153017
          </a>
        </div>
        <span class="text-xs text-gray-500">Click to chat on WhatsApp</span>
      </div>

      <!-- Desktop Menu -->
      <div class="hidden md:flex space-x-8 font-medium">
        <NuxtLink to="/about" class="hover:text-yellow-500 transition">About</NuxtLink>
        <NuxtLink to="/contact" class="hover:text-yellow-500 transition">Contact</NuxtLink>
      </div>

      <!-- Mobile Menu Button -->
      <button
        @click="isOpen = !isOpen"
        class="md:hidden text-2xl text-gray-700 focus:outline-none"
      >
        <span v-if="!isOpen">☰</span>
        <span v-else>✕</span>
      </button>
    </div>

    <!-- Mobile Menu -->
    <div v-if="isOpen" class="md:hidden bg-white border-t shadow-md">
      <div class="flex flex-col space-y-4 p-4 font-medium text-center">

        <!-- Mobile WhatsApp Numbers -->
        <div class="flex flex-col space-y-2 text-gray-700 font-semibold">
          <a href="https://wa.me/2348023190606" target="_blank" class="hover:text-green-600">08023190606</a>
          <a href="https://wa.me/2347084440011" target="_blank" class="hover:text-green-600">07084440011</a>
          <a href="https://wa.me/2348037153017" target="_blank" class="hover:text-green-600">08037153017</a>
          <span class="text-xs text-gray-500">Tap to open WhatsApp</span>
        </div>

        <NuxtLink to="/about" class="hover:text-yellow-500" @click="isOpen = false">About</NuxtLink>
        <NuxtLink to="/contact" class="hover:text-yellow-500" @click="isOpen = false">Contact</NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'
const isOpen = ref(false)
</script>
