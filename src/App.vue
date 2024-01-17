<script setup>
import { ref } from 'vue';
import JSConfetti from 'js-confetti'
import ChildComp from './components/ChildComp.vue'


const confetti = new JSConfetti()

function showConfetti() {
  confetti.addConfetti()
}

const greating = ref('Hello du parent');
const childMsg = ref('Pas encore de message de l\'enfant')

showConfetti()
</script>

<template>

  <h1 @click="showConfetti">🎉 Félicitations!</h1>
  <!-- <ChildComp @response="(msg) => childMsg = msg" :msg="greating"/> -->
  <ChildComp>
    {{ greating }}
  </ChildComp>
  <p>{{ childMsg }}</p>


</template>

<style scoped>
h1 {
  text-align: center;
  cursor: pointer;
  margin-top: 3em;
}
</style>