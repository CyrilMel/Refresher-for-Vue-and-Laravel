<template>
  <div>
    <h2>Login Demo</h2>

    <p v-if="isLoggedIn">You are logged in</p>
    <p v-else>Please log in</p>

    <button @click="toggleLogin">
      Toggle Login
    </button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isLoggedIn = ref(false)

function toggleLogin() {
  isLoggedIn.value = !isLoggedIn.value
}
</script>