<template>
  <div>
    <h1>Vue 3 Composition API Demos</h1>

    <CounterDemo />
    <hr>
    <ListDemo />
    <LoginDemo />
    <InputDemo />
  </div>
</template>

<script setup>
import CounterDemo from './components/CounterDemo.vue'
import ListDemo from './components/ListDemo.vue'
import LoginDemo from './components/LoginDemo.vue'
import InputDemo from './components/InputDemo.vue'
</script>
