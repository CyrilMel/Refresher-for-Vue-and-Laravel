<template>
  <div class="p-3 border rounded">
    <h2 class="text-primary">Counter Demo</h2>
    <p>Count: {{ count }}</p>
    <button class="btn btn-success me-2" @click="increment">Increase</button>
    <p>{{ isEven ? 'Even' : 'Odd' }}</p>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue'

const count = ref(0)

// method
function increment() {
  count.value++
}

// computed
const isEven = computed(() => count.value % 2 === 0)
</script>