<template>
  <div class="text-center border-b-2 border-dashed border-gray-300 pb-4">
    <h1 class="text-2xl font-bold uppercase tracking-wider">DEVELOPER RECEIPT</h1>
    <p class="text-sm mt-2">Order #: DEV-{{ currentYear }}</p>
    <p class="text-sm">{{ currentDate }}</p>
  </div>
</template>

<script setup lang="ts">
const currentYear = new Date().getFullYear()
const currentDate = new Date().toLocaleDateString()
</script>