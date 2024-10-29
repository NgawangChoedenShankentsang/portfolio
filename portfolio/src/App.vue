<template>
  <div class="min-h-screen bg-gray-100 py-8 px-4">
    <div class="receipt max-w-md mx-auto bg-white p-6">
      <Header />
      <Bio />
      <Skills />
      <Projects />
      <Achievements />
      <Contact />
    </div>
  </div>
</template>

<script setup lang="ts">
import Header from './components/Header.vue'
import Bio from './components/Bio.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Achievements from './components/Achievements.vue'
import Contact from './components/Contact.vue'
</script>