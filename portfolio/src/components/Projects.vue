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

<script setup lang="ts">
const projects = [
  {
    name: 'E-commerce Platform',
    description: 'Full-stack shopping platform',
    tech: 'Vue.js, Node.js, MongoDB',
    price: '2,500'
  },
  {
    name: 'Weather Dashboard',
    description: 'Real-time weather tracking',
    tech: 'Vue.js, OpenWeather API',
    price: '1,200'
  },
  {
    name: 'Task Manager',
    description: 'Collaborative project tool',
    tech: 'Vue.js, Firebase',
    price: '1,800'
  }
]
</script>