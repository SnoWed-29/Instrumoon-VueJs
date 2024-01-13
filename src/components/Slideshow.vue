<script setup>
import { RouterLink, RouterView } from 'vue-router'


import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'
const slides = [
  {
    title: 'Slide #1',
    content: 'hhh'
  },
  {
    title: 'Slide #2',    
    content: 'hhh'

  }, 
  {
    title: 'Slide #1',
    content: 'hhh'
  },
  {
    title: 'Slide #2',    
    content: 'hhh'

  },
]
</script>

<template>
  <vueper-slides>
  <vueper-slide
    v-for="(slide, i) in slides"
    :key="i"
    :title="slide.title"
    :content="slide.content">
  </vueper-slide>
</vueper-slides>
</template>
