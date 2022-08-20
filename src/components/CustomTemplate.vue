<script setup>
defineProps({
  customMessage: {
    type: String,
    required: true,
  },
});
let message = "My Message";

let htmlSyntex = '<span style="color:red;">This color should be in red</span>';
</script>

<template>
<p>{{ message }}</p>

<p>This should not render html</p>
<div>{{htmlSyntex}}</div>
<p>This should render the red span, because of the <strong>v-html</strong></p>
<div v-html="htmlSyntex"></div>
</template>