<script setup lang="ts">
import Navbar from './components/Navbar.vue';
import Home from './views/Home.vue';
import About from './views/About.vue';
import Projects from './views/Projects.vue';
import Contact from './views/Contact.vue'
</script>

<template>
  <Navbar/>
  
  <div id="home" class="area">
    <Home />
  </div>

  <div id="about" class="area">
    <About />
  </div>

  <div id="projects" class="area">
    <Projects />
  </div>

  <div id="contact" class="area">
    <Contact />
  </div>
</template>

<style scoped>
.area {
  min-height: 100vh;
  padding-top: 6rem;
}
</style>
