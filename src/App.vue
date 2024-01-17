<script setup>
import { ref } from 'vue';
import ChildComp from './components/ChildComp.vue'

const greating = ref('Hello du parent');
</script>

<template>
  <ChildComp :msg="greating"/>
</template>

<style scoped>

</style>