<template>
  <div class="border-b-2 border-dashed border-gray-300 py-4">
    <h2 class="font-bold mb-2">SKILLS INVENTORY:</h2>
    <div v-for="skill in skills" :key="skill.name" class="flex justify-between text-sm my-1">
      <span>{{ skill.name }}</span>
      <span class="font-mono">{{ skill.level }}</span>
    </div>
  </div>
</template>

<script setup>
const skills = [
  { name: 'Symfony PHP', level: '[--/////////////]' },
  { name: 'TypeScript', level: '[------/////////]' },
  { name: 'Vue.js', level: '[-----//////////]' },
  { name: 'Git', level: '[--/////////////]' },
  { name: 'Tailwind', level: '[-----//////////]' },
]
</script>