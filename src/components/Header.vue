<template>
  <div class="text-center border-b-2 border-dashed border-gray-300 pb-4">
    <h1 class="text-2xl font-bold uppercase tracking-wider">DEVELOPER RECEIPT</h1>
    <p class="text-sm mt-2">Order #: DEV-{{ currentYear }}</p>
    <p class="text-sm">{{ currentDate }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const currentYear = new Date().getFullYear()
const currentDate = formatDate(new Date())

function formatDate(date) {
  const day = String(date.getDate()).padStart(2, '0') // Ensure two digits
  const month = String(date.getMonth() + 1).padStart(2, '0') // Months are zero-indexed
  const year = date.getFullYear()
  return `${day}/${month}/${year}`
}
</script>
