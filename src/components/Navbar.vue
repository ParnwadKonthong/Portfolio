<script setup lang="ts">
import { ref, onMounted } from 'vue'

const currentSection = ref('home')

const sections = ['home', 'about', 'projects', 'contact']

const changeSection = (id: string) => {
  const el = document.getElementById(id)
  if (el) {
    el.scrollIntoView({ behavior: 'smooth' })
  }
}


let observer: IntersectionObserver

onMounted(() => {
  observer = new IntersectionObserver(
    (entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          currentSection.value = entry.target.id
        }
      })
    },
    {
      threshold: 0.5, 
    }
  )

  sections.forEach(id => {
    const el = document.getElementById(id)
    if (el) observer.observe(el)
  })
})

</script>

<template>
  <div class="flex justify-between w-full p-8 fixed top-0 left-0 bg-white z-50 shadow">
    <div class="font-bold">PORTFOLIO</div>
    <div class="flex space-x-12 ml-auto cursor-pointer">
      <a
        v-for="id in sections"
        :key="id"
        @click="changeSection(id)"
        :class="currentSection === id ? 'font-bold' : ''"
      >
        {{ id.charAt(0).toUpperCase() + id.slice(1) }}
      </a>
    </div>
  </div>
</template>

<style scoped>
a {
  transition: all 0.3s ease;
}
</style>
