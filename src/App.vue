<script setup>
import { ref } from 'vue';

// Déclaration d'une référenche de chaîne
const count = ref(0);

// Met à jour le state du component
function increment() {
  count.value+=2; // Ajout de 2 à chaque click à la variable count
}

</script>

<template>
  <!-- Rendez ce bouton fonctionnel -->
  <button @click="increment">
    count à : {{ count }}
  </button>
</template>

<style scoped>
.title {
  color: red;
}
</style>