<template>
<section class="relative bg-yellow-400 py-14 overflow-hidden">
  <!-- Background Image & Shapes -->
  <div class="absolute inset-0 opacity-10 bg-[url('https://i.imgur.com/ajPeT3I.png')] bg-cover bg-center"></div>
  <div class="absolute -top-10 -left-10 w-40 h-40 bg-gray-900 rotate-45 opacity-20"></div>
  <div class="absolute -bottom-10 -right-10 w-40 h-40 bg-red-600 rotate-45 opacity-20"></div>

  <div class="relative container mx-auto px-6 text-center">
    <!-- Header -->
    <h2 class="text-4xl md:text-5xl font-black text-gray-900 tracking-wide drop-shadow-sm">
      CONTACT US
    </h2>

    <p class="text-lg md:text-xl font-semibold text-gray-800 mt-3">
      Enquiries:
      <span class="text-gray-900">08023190606</span> |
      <span class="text-gray-900">08037153638</span> |
      <span class="text-gray-900">08037153017</span>
    </p>

    <!-- Contact Buttons -->
    <div class="mt-8 flex flex-wrap justify-center gap-5">
      <a href="tel:08023190606"
         class="flex items-center gap-2 bg-gray-900 text-white px-8 py-3 rounded-full font-bold shadow-lg hover:bg-gray-800 transition transform hover:scale-105">
        <span>📞</span> Call Now
      </a>

      <a href="https://wa.me/2348023190606"
         class="flex items-center gap-2 bg-green-600 text-white px-8 py-3 rounded-full font-bold shadow-lg hover:bg-green-500 transition transform hover:scale-105">
        <span>💬</span> WhatsApp
      </a>

      <a href="mailto:info@yourworkshop.com"
         class="flex items-center gap-2 bg-red-600 text-white px-8 py-3 rounded-full font-bold shadow-lg hover:bg-red-500 transition transform hover:scale-105">
        <span>✉️</span> Email Support
      </a>
    </div>

    <!-- Offices Info -->
    <div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-10 text-left">
      <!-- Lagos Office -->
      <div class="bg-white/20 backdrop-blur-md p-6 rounded-2xl shadow-lg border border-white/20">
        <h3 class="text-2xl font-bold text-gray-900 mb-3">Lagos Office</h3>
        <p class="text-gray-900 font-semibold mb-1">📍 20 Akinremi St., Anifowose, Ikeja, Lagos</p>
        <p class="text-gray-900 mb-1">📞 08037153638</p>
        <p class="text-gray-900">📞 08023190606</p>
      </div>

      <!-- Abuja Office -->
      <div class="bg-white/20 backdrop-blur-md p-6 rounded-2xl shadow-lg border border-white/20">
        <h3 class="text-2xl font-bold text-gray-900 mb-3">Abuja Office</h3>
        <p class="text-gray-900 font-semibold mb-1">📍 AJB Mall, Plot 1123, Oladipo Diya Road, Gudu District, Abuja</p>
        <p class="text-gray-900 mb-1">📞 08070447698</p>
        <p class="text-gray-900">📞 08101033337</p>
      </div>
    </div>
  </div>
</section>
</template>