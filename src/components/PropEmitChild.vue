<template>
    <div>
        <h3>{{  message  }}</h3>

        <button @click="emitEvent">Send Message</button>
    </div>
</template>

<script setup>
defineProps({
    message: 'message from parent component!'
});

const emit = defineEmits(['updateMessage']);

const emitEvent = () => {
    emit('updateMessage', 'New message from the child component!');
}

</script>