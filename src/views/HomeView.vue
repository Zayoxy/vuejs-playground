<script setup>
import { ref } from "vue";

// Composition API (The new one)
// Data

const counter = ref(0);
// Methods

function increment() {
  counter.value++;
}

// Computed properties
// Lifecycle hooks
// --------------------------------------------------
</script>

<template>
  <h1>Welcome to my website's homepage</h1>
  <h3>Our battle will be legendary!</h3>

  <button @click="increment">Click me! {{ counter }}</button>
</template>

<!--
<script>
export default {
  // Option API (The old way to build VueJS apps)
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    increment() {
      this.counter++;
    },
  },
  // --------------------------------------------------
};
</script>
-->

<style scoped>
button {
  background-color: rgb(102, 102, 102);
  font-size: 15px;
  border: 2px solid white;
  color: white;
}
</style>
