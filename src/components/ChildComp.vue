<template>
    <h2>Un composant enfant!</h2>
    <p>{{ msg || 'Aucune prop passée pour le moment'}}</p>
</template>

<script setup>
const props = defineProps({
    msg: String
})

// Declare les évènements émis
const emit = defineEmits(['response'])

// emit avec un argument
emit('response', "hello à partir de l'enfant")
</script>