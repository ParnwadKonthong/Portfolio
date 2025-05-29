<script setup lang="ts">
import { ref, onMounted } from "vue";

const currentSection = ref("home");
const menuOpen = ref(false)

const sections = ["home", "about", "projects", "contact"];

const changeSection = (id: string) => {
  const el = document.getElementById(id);
  if (el) {
    el.scrollIntoView({ behavior: "smooth" });
    menuOpen.value = false
  }
};

let observer: IntersectionObserver;

onMounted(() => {
  observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          currentSection.value = entry.target.id;
        }
      });
    },
    {
      threshold: 0.5,
    }
  );

  sections.forEach((id) => {
    const el = document.getElementById(id);
    if (el) observer.observe(el);
  });
});
</script>

<template>
  <div
    class="flex justify-between w-full p-4 fixed top-0 left-0 bg-white/99 z-50 shadow"
  >
    <div class="font-bold text-2xl">PORTFOLIO</div>
    <div class="flex space-x-12 ml-auto cursor-pointer text-lg">
      <button
        class="md:hidden text-3xl mr-auto focus:outline-none cursor-pointer"
        @click="menuOpen = !menuOpen"
      >
        ☰
      </button>

      <div class="hidden md:flex space-x-12 text-lg">
        <a
          v-for="id in sections"
          :key="id"
          @click="changeSection(id)"
          :class="currentSection === id ? 'font-bold' : ''"
        >
          {{ id.charAt(0).toUpperCase() + id.slice(1) }}
        </a>
      </div>

      <div
        v-if="menuOpen"
        class="absolute right-0 top-12 w-36 p-4 bg-white/99 shadow-lg rounded-xl z-50 flex flex-col space-y-4 lg:hidden"
      >
        <a
          v-for="id in sections"
          :key="'mobile-' + id"
          @click="changeSection(id)"
          :class="[
            'cursor-pointer hover:font-bold transition',
            currentSection === id ? 'font-bold' : '',
          ]"
        >
          {{ id.charAt(0).toUpperCase() + id.slice(1) }}
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
a {
  transition: all 0.3s ease;
}
</style>
