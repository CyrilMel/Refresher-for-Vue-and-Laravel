<template>
  <div>
    <h1>Emit Example</h1>

    <!-- Display received message -->
    <p><strong>Message from Child:</strong> {{ receivedMessage }}</p>

    <!-- Child component -->
    <Child @sendMessage="handleMessage" />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Child from './Child.vue';
// state to store message from child
const receivedMessage = ref('')

// function to handle emitted data
function handleMessage(message) {
  receivedMessage.value = message
}
</script>