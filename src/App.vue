<script setup>
import { ref } from 'vue';
import ChildComp from './components/ChildComp.vue'

const greating = ref('Hello du parent');
const childMsg = ref('Pas encore de message de l\'enfant')
</script>

<template>
  <ChildComp @response="(msg) => childMsg = msg" :msg="greating"/>
  <p>{{ childMsg }}</p>
</template>

<style scoped>

</style>