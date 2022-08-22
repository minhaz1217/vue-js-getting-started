<script setup>
import { ref } from 'vue'

const emit = defineEmits(['response']);

const childMsg = ref('No child msg yet')
emit('response', "Hello From the Child");
</script>

<template>
  <p>{{ "Child Mounted" }}</p>
</template>