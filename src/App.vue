<script setup>
import { ref } from 'vue';

import { onMounted } from 'vue';

const pElementRef = ref(null);

onMounted(() => {
  // le composant est maintenant monté
  pElementRef.value.textContent = "monté !";
})

</script>

<template>
  <p ref="pElementRef">hello</p>
</template>

<style scoped>

</style>