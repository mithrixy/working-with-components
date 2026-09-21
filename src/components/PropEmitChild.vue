<script setup>
defineProps({
    message: String
});

const emit = defineEmits(['updateMessage']);

const emitEvent = () => {
    emit('updateMessage', 'New message from the child component!');
}

</script>

<template>
    <p> Child message: {{ message }} </p>
    <button @click="emitEvent">Update Message</button>
</template>
