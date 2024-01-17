<script setup>
import { ref } from 'vue';

// Déclaration d'une référenche de chaîne
const message = ref('Hello World');

const titleClass = ref('title')

</script>

<template>
  <h1 :id="dynamicId" :class="titleClass">Passez moi en rouge</h1>
  <p>{{ titleClass }}</p>
</template>

<style scoped>
.title {
  color: red;
}
</style>