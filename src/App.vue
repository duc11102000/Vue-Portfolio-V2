<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');

body {
  margin: 0;
  font-family: "Inter", sans-serif;
}

html {
  scroll-behavior: smooth;
}

section {
  padding-top: 4vh;
  /* height: 96vh; */
  margin: 0 5rem;
  box-sizing: border-box;
  min-height: fit-content;
}
</style>
