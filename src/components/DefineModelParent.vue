<template>
    <DefineModelChild v-model="message"/>
    <p> Current message: {{ message }} </p>
</template>

<script setup>
import { ref } from 'vue';
import DefineModelChild from './DefineModelChild.vue';

const message = ref('');
</script>