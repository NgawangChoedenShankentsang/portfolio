<template>
  <div class="border-b-2 border-dashed border-gray-300 py-4">
    <h2 class="font-bold mb-2">PROJECT ITEMS:</h2>
    <div v-for="project in projects" :key="project.name" class="mb-3">
      <div class="flex justify-between text-sm">
        <span class="font-bold">{{ project.name }}</span>
        <span>${{ project.price }}</span>
      </div>
      <p class="text-xs text-gray-600">{{ project.description }}</p>
      <p class="text-xs text-gray-500">Stack: {{ project.tech }}</p>
    </div>
  </div>
</template>

<script setup>
const projects = [
  {
    name: 'License Management Tool (LMT)',
    description: 'Tool for managing software licenses.',
    tech: 'Symfony 6.4, MySQL',
    price: '3,000'
  },
  {
    name: 'Bg-Remove Tool',
    description: 'Removing backgrounds from images.',
    tech: 'Vue.js, @imgly/background-removal',
    price: '1,500'
  },
  {
    name: 'Himalaya Imbiss',
    description: 'POS system for our Imbiss.',
    tech: 'Vite, TypeScript, TW CSS',
    price: '2,200'
  }
]
</script>
