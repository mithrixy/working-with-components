<script setup>
import PropEmitChild from './PropEmitChild.vue'
import { ref } from 'vue';

const message = ref('Message from the parent');

const handleMessage = (newMessage) => {
    message.value = newMessage;
}

</script>

<template>
    <PropEmitChild :message="message" @updateMessage="message = $event"/>
    <p> Parent message: {{  message  }}</p>
</template>
