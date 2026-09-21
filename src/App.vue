<script setup>
import PropEmitChild from './components/PropEmitChild.vue';
import PropEmitParent from './components/PropEmitParent.vue';
import DefineModelChild from './components/DefineModelChild.vue';
import DefineModelParent from './components/DefineModelParent.vue';
</script>

<template>
<div>
  <h3>Working with Components</h3>
</div>

<PropEmitParent></PropEmitParent>
<DefineModelParent></DefineModelParent>
</template>
