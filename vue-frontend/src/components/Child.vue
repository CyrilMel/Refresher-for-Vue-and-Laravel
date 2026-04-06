<template>
  <div class="border p-3 mt-3">
    <h3>Child Component</h3>

    <!-- Input to send data -->
    <input v-model="message" placeholder="Type a message" />

    <!-- Button triggers emit -->
    <button @click="sendMessage">
      Send to Parent
    </button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// local state
const message = ref('')

// define emit
const emit = defineEmits(['sendMessage'])

// function to emit data
function sendMessage() {
  emit('sendMessage', message.value)
  message.value = '' // clear input
}
</script>