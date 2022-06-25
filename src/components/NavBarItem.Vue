<script setup>
defineProps({
  Text: {
    type: String,
    required: true
  },
  Link: {
    type: String,
    required: true
  }
})
</script>
<template>
  <li><a href="{{ Link }}"> {{ Text }}</a></li>
</template>

<style scoped>
</style>
