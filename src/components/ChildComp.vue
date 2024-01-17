<template>
    <h2>Un composant enfant!</h2>
    <p>{{ msg || 'Aucune prop passée pour le moment'}}</p>
</template>

<script setup>
const props = defineProps({
    msg: String
})
</script>