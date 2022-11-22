<script setup>
import { ref } from "vue";
const counter = ref(0);
</script>

<template>
  <h1>Welcome to my website's homepage</h1>
  <h3>Our battle will be legendary!</h3>

  <button @click="counter++">Click me! {{ counter }}</button>
</template>

<style scoped>
button {
  background-color: rgb(102, 102, 102);
  font-size: 15px;
  border: 2px solid white;
  color: white;
}
</style>
