<template>
<div class="bg-gray-50 text-gray-900 font-sans">
  <section class="relative h-[85vh] flex items-center bg-gradient-to-br from-gray-900 via-gray-800 to-red-900 overflow-hidden px-6 sm:px-10">

    <!-- Image Left -->
    <div class="relative z-10 w-[45%] flex justify-center">
      <img 
        src="/assest/sb-.png" 
        alt="Spray Booth"
        class="w-[350px] sm:w-[450px] md:w-[520px] object-contain drop-shadow-2xl"
      />
    </div>

    <!-- Text Right -->
    <div class="relative z-10 w-[55%] pr-6 sm:pr-12 text-right">
      <h1 class="text-4xl sm:text-5xl font-bold text-white leading-tight">
        Modern <span class="text-red-500">Spray Booth</span> Technology
      </h1>
      <p class="mt-4 text-gray-300 text-lg">
        High-performance automotive spray booth engineered for efficiency, durability and premium finishing.
      </p>
      
    </div>
  </section>
</div>

  
 <section class="py-24 bg-gray-50">
  <div class="container mx-auto px-6 max-w-7xl">
  <div class="text-center max-w-4xl mx-auto mb-12 px-4">
  <h2 class="text-3xl md:text-4xl font-extrabold text-gray-800 leading-snug">
    For your 
    <span class="text-yellow-500">Garage Equipment</span>, 
    <span class="text-yellow-500">Automotive Diagnostics Tools</span>, 
    <span class="text-yellow-500">Spraybooth (Car Oven)</span>, 
    <span class="text-yellow-500">Car Wash Equipment</span> 
    and 
    <span class="text-yellow-500">Garage Set Up</span>
  </h2>

  <div class="mt-4 w-28 h-1 bg-yellow-500 mx-auto rounded"></div>
</div>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
      <a
        v-for="item in assest"
        :key="item.name"
        :href="item.link"
        target="_blank"
        class="block bg-white shadow-md rounded-lg overflow-hidden hover:shadow-lg transition mx-auto w-full max-w-sm"
      >
        <img
          :src="item.image"
          :alt="item.name"
          class="w-full h-48 object-contain bg-gray-100"
        />
        <div class="p-4">
          <h3 class="text-lg font-semibold text-gray-700">{{ item.name }}</h3>
          <p class="text-sm text-gray-500 mt-1">{{ item.description }}</p>
        </div>
      </a>
    </div>
  </div>
</section>
  
</template>


<script setup>
const assest = [
{
  name: "Automotive Spray Booth",
  image: "/assest/sb-.png",
  description: "Sealed and controlled environment designed for high-quality vehicle painting, ensuring dust-free finishing and proper drying.",
  link: "http://garutech.ng/product/3St44j49bl7hpbDJAJgO"
},
{
  name: "2 Post Lift",
  image: "/assest/2post lift.webp",
  description: "Professional vehicle lift ideal for repairs and maintenance. It provides safe, secure, and efficient under-body access.",
  link:"http://garutech.ng/product/a9Oeuo05oiphvWz5nz72"
},
{
  name: "Wheel Balancer",
  image: "/assest/balancer.jpg",
  description: "A machine used to balance the weight distribution of car wheels, ensuring smooth rotation and reducing tire vibration.",
  link:"http://garutech.ng/product/eOt6ImIxDLBLRb1qvVon"
},
{
  name: "4 Post Lift",
  image: "/assest/4 Post lift.jpg",
  description: "A stable, drive-on style vehicle lift used for alignment, repairs, and long-term vehicle storage with maximum lifting safety.",
  link:"http://garutech.ng/product/oF5UI1lxOhPa2uvtgm4u"
},
{
  name: "Tyre Changer",
  image: "/assest/tyre ch.jpg",
  description: "A specialized machine used to mount and dismount tires from wheel rims quickly, safely, and without damage.",
  link:"http://garutech.ng/product/EPRfU3idTyIaVW29H2rQ"
},
{
  name: "3D Wheel Alignment Machine",
  image: "/assest/al.png",
  description: "It is a precision system that uses advanced 3D imaging to measure wheel angles and ensure accurate alignment for better vehicle handling.",
  link:"http://garutech.ng/product/gp2OoWe2uYPXAuVBGjef"
}


];
</script>

