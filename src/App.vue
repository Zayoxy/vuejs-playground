<template>
  <header>
    <NavBar />
  </header>

  <RouterView />
</template>

<script>
import { RouterView } from "vue-router";
import NavBar from "@/components/NavBar.vue";

export default {
  data() {
    return {
      counter: 0,
    };
  },
};
</script>

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
