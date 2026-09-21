<script setup>
import { ref } from 'vue';
import DefineModelChild from './DefineModelChild.vue';

const message = ref('Initial value');
</script>

<template>
    <DefineModelChild v-model="message"/>
    <p> Parent sees: {{ message }} </p>
</template>
