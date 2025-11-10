<template>
   <div class="bg-gray-50 text-gray-900 font-sans">
    <section class="relative h-[85vh] bg-[url('/assest/spray-.png')] bg-cover bg-center flex items-center justify-center">
  <div class="absolute inset-0 bg-gradient-to-br from-black/70 via-black/50 to-red-900/40 animate-pulse"></div>
  <div class="absolute bottom-0 w-full overflow-hidden leading-[0] rotate-180">
    <svg class="relative block w-full h-16 sm:h-24 text-white" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none" viewBox="0 0 1200 120">
      <path d="M321.39,56.9C161.16,77,0,119.5,0,119.5V0H1200V119.5s-161.16-42.5-321.39-62.6C720.92,36.4,600,67.2,479.08,67.2,358.16,67.2,321.39,56.9,321.39,56.9Z" class="fill-white"></path>
    </svg>
  </div>

 <div class="relative z-10 text-center px-6 sm:px-12 py-8 rounded-3xl backdrop-blur-md bg-white/10 border border-white/20 shadow-2xl max-w-3xl animate-fade-in">
    <h1 class="text-4xl sm:text-5xl md:text-6xl font-extrabold text-white leading-tight drop-shadow-lg">
       <span class="text-red-500">Modern SprayBooth</span>
    </h1>
  </div>
</section></div>

  
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
  image: "/assest/spray-.png",
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

