<script setup>
const message = defineModel({ type: String});
</script>

<template>
    <input v-model="message" placeholder="child msg"/>
</template>

