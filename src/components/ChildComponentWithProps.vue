<script setup>
const props = defineProps({
  msg: String
});
</script>

<template>
    <h1>{{ msg || "Hi"}}</h1>
</template>