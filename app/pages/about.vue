<template>
  <section class="relative bg-gray-50 py-24">
  <!-- Decorative curved top -->
  <div class="absolute top-0 w-full overflow-hidden leading-[0]">
    <svg class="relative block w-full h-16 sm:h-24 text-gray-50" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none" viewBox="0 0 1200 120">
      <path d="M321.39,56.9C161.16,77,0,119.5,0,119.5V0H1200V119.5s-161.16-42.5-321.39-62.6C720.92,36.4,600,67.2,479.08,67.2,358.16,67.2,321.39,56.9,321.39,56.9Z" class="fill-current"></path>
    </svg>
  </div>

  <div class="container mx-auto px-6 relative z-10">
    <div class="flex flex-col md:flex-row items-center gap-12 md:gap-24">
      
      <!-- Image / Hero -->
      <div class="md:w-1/2">
        <img src="/assest/spray-.png" alt="Automobile Workshop" class="rounded-3xl shadow-2xl object-cover w-full h-full">
      </div>

      <!-- Content -->
      <div class="md:w-1/2 text-center md:text-left">
        <h2 class="text-4xl font-extrabold text-gray-900 mb-6 drop-shadow-md">
          About <span class="text-red-500">Us</span>
        </h2>
        <p class="text-gray-700 text-lg leading-relaxed mb-6">
          Garu Tech is a leading supplier of premium garage and automotive workshop equipment in Nigeria. 
          We specialize in providing complete solutions for modern auto garages, including vehicle lifts, 
          spray booths (car ovens), diagnostic tools, car wash systems, wheel alignment machines, tyre service
           equipment, and full workshop setup consulting.
        </p>
        <p class="text-gray-700 text-lg leading-relaxed mb-6">
          With a strong commitment to quality, reliability, and after-sales support, we help mechanics, auto centers,
           technical schools, and industrial workshops build efficient and professional service environments.</p>
            
           <p class="text-gray-700 text-lg leading-relaxed mb-6">
            Our team ensures equipment is properly installed, tested, and supported, so customers can operate with
             confidence and deliver excellent automotive services.
        </p>

        <NuxtLink to="/contact" class="inline-block bg-red-500 text-white px-8 py-3 rounded-full shadow-lg font-semibold hover:bg-red-600 transition transform hover:scale-105">
          Get in Touch
        </NuxtLink>
      </div>

    </div>
  </div>
</section>
</template>

<script setup>
</script>
