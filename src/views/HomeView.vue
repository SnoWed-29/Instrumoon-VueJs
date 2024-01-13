<script setup>
import { RouterLink, RouterView } from 'vue-router'

import Navbar from '../components/Navbar.vue';
import Hero from '../components/Hero.vue';
import Svg from '../components/Svg.vue';
</script>

<template>
  <Svg />
  <Navbar />
  <Hero />
  <main class="w-9/12 mx-auto flex justify-between space-x-3 my-6">
    <!-- Filter -->
    <div class="w-1/3 bg-[#ffffff25] h-20">

    </div>
    <!-- showCase -->
    <div class="w-2/3 font-medium">
      <div class="flex flex-col space-y-3" >
       <div class="flex w-full px-2 space-x-2">
          <!-- Item 01 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25]  shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 02 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 03 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
       </div>
       <div class="flex w-full px-2 space-x-2">
          <!-- Item 01 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25]  shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 02 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 03 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
       </div><div class="flex w-full px-2 space-x-2">
          <!-- Item 01 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25]  shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 02 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
          <!-- Items 03 -->
          <div class="flex w-1/3 py-3 px-2 rounded-md bg-[#ffffff25] shadow-xl"  >
            <div class="flex flex-col w-full items-center">
              <div class="flex w-full justify-center">
                <img src="../assets/images/02.jpg" class="w-[200px] mx-auto">
              </div>
              <div class="flex w-full my-1 p-1">
                <h2 class="text-xl w-fit mx-auto">Lorem, ipsum.</h2>
              </div>
              <div class="flex w-full">
                <a href="#" class="bg-[#CFFDF8] text-black border border-[#216583] hover:bg-[#216583] hover:border-[#CFFDF8] w-full text-center text-xl px-4 py-2">Buy</a>
              </div>
            </div>
          </div>
       </div>
      </div>
    </div>
  </main>
<!-- https://antoniandre.github.io/vueper-slides/?ref=madewithvuejs.com -->
</template>
