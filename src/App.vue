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

<style>
.area {
  padding-top: 6rem;
  padding-left: 6rem;
  padding-right: 6rem;
}

body {
  font-family: 'Exo 2', serif;
  margin: 0;
  min-height: 100vh;
  background: linear-gradient(
    135deg, /* มุมเอียงจากบนซ้ายไปล่างขวา */
    #ffd1dc,  /* pastel pink */
    #ffe4b5,  /* pastel peach */
    #fffac8,  /* pastel yellow */
    #d5f4e6,  /* pastel mint */
    #add8e6,  /* pastel blue */
    #d0bdf4,  /* pastel purple */
    #f3c6ff   /* pastel lavender */
  );
}

@media (max-width: 1440px) {
  .area {
    padding-left: 4rem;
    padding-right: 4rem;
  }
  body {
    font-size: 17px;
  }
}

@media (max-width: 1024px) {
  .area {
    padding-left: 3rem;
    padding-right: 3rem;
  }
  body {
    font-size: 16px;
  }
}

@media (max-width: 768px) {
  .area {
    padding-left: 2rem;
    padding-right: 2rem;
  }
  body {
    font-size: 15px;
  }
}

@media (max-width: 480px) {
  .area {
    padding-left: 1rem;
    padding-right: 1rem;
  }
  body {
    font-size: 14px;
  }
}

</style>
