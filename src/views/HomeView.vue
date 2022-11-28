<template>
  <h1>Welcome to my website's homepage</h1>
  <h3>Our battle will be legendary!</h3>

  <p ref="p">My name is {{ name }} and I am {{ age }} years old</p>
  <button @click="handleClick()">Click on me you dummy !</button>

  <!-- <button @click="increment">Click me! {{ counter }}</button> -->
</template>

<script>
import { ref } from "vue";

export default {
  name: "HomeView",
  setup() {
    let name = "Alexandre";
    let age = 18;

    const p = ref(null);
    console.log(p); // Will log "Undefined" cuz it hasn't been returned yet

    const handleClick = () => {
      console.log(p.value.classList); // Works here, cuz when we click the button, the p ref is already set
      p.value.classList.add("test");
      p.value.textContent = "Hello froggies :D";
    };

    return { name, age, handleClick, p }; // We have to return the function we want to display cuz they ain't reactive
  },
  // created() {
  //   console.log("Created");
  // },
  // mounted() {
  //   console.log("Mounted");
  // },
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
