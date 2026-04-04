<template>
  <div>
    <h2>Input Demo</h2>
    <input v-model="name" placeholder="Enter your name" />
    <p>Hello, {{ name }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// reactive state
const name = ref('')
</script>