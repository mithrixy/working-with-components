<template>
    <div>
        <input v-model="message" placeholder="Type here..."/>
    </div>
</template>

<script setup>
//receive + modify message property
const message = defineModel();
</script>