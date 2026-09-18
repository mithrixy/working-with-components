<template>
    <PropEmitChild :message="message"/>
    <PropEmitChild @updateMessage="handleMessage"/>
    <p>Message from child component: {{  message  }}</p>
</template>

<script setup>
import PropEmitChild from './PropEmitChild.vue'
import { ref } from 'vue';

const message = ref('');

const handleMessage = (newMessage) => {
    message.value = newMessage;
}

</script>