<template>
  <h1>Welcome to my website's homepage</h1>
  <h3>Our battle will be legendary!</h3>

  <button @click="increment()">Click me! {{ counter }}</button>
</template>

<script>
export default {
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
};
</script>

<style scoped>
button {
  background-color: rgb(102, 102, 102);
  font-size: 15px;
  border: 2px solid white;
  color: white;
}
</style>
