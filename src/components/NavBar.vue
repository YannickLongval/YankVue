<script setup>
defineProps({
  NavTitle: {
    type: String,
    required: true
  }
})
</script>
<template>
  <h1>{{ NavTitle }}</h1>
  <ul id="links">
    <slot></slot>
  </ul>
</template>

<style scoped>
    
    * {
        background-color: var(--vt-c-text-dark-2);
    }
</style>
