<script setup lang="ts">
import { ref } from "vue";
import HelloWorld from "./components/HelloWorld.vue";
import MyButton from "./components/MyButton.vue";

const count = ref(0);
</script>

<template>
  <div>
    <MyButton @update:count="count++"> count is: {{ count }} </MyButton>
    <HelloWorld msg="Vite + Vue" />
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
