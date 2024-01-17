<script setup>
import { ref } from 'vue';

const message = ref('Hello World');

</script>

<template>
  <h1>Rendez moi dynamique</h1>
  <p>{{ message.split('').reverse().join('') }}</p>
</template>