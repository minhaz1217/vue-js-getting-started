<script setup>
import { onMounted, onUnmounted, ref } from 'vue'

const p = ref(null);

onMounted( ()=>{
    p.value.textContent = "Hello World";
    // console.log(p.value);
});
onUnmounted(()=>{
    console.log("Component Unmounted");
});
</script>

<template>
  <p ref="p">hello</p>
</template>