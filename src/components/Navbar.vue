<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="fixed top-0 z-10 w-full bg-[#ffffff25] border-b-2 border-b-[#F76262] text-white">
      <nav class="w-9/12 mx-auto p-3 flex justify-between  ">
        <RouterLink to="/"  class="text-xl font-bold p-2">Home</RouterLink>
        <RouterLink to="/about" class="text-xl font-bold p-2">About</RouterLink>
        <RouterLink to="/about" class="text-xl font-bold p-2">About</RouterLink>
        <RouterLink to="/about" class="text-xl font-bold p-2">About</RouterLink>
        <RouterLink to="/about" class="text-xl font-bold p-2">About</RouterLink>
      </nav>
    </div>
  </header>
</template>