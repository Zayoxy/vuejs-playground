<script setup>
import { RouterLink, RouterView } from "vue-router";
import NavBar from "@/components/NavBar.vue";
</script>

<template>
  <header>
    <NavBar />
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
}
</style>
