<script setup>
import { ref } from 'vue'

import PropEmitChild from './components/PropEmitChild.vue';
import DefineModelChild from './components/DefineModelChild.vue';

const message = ref('message from')
const modelMessage = ref('Type here...')
</script>

<template>
  <h1>Task 1 — defineProps / defineEmits</h1>
  <h2> Parent: {{ message }}</h2>
  <PropEmitChild :message="message" @update-message="message = $event" />

  <hr />

  <h1>Task 2 — defineModel</h1>
  <DefineModelChild v-model="modelMessage" />
  <p> Parent sees: {{ modelMessage }}</p>
</template>
