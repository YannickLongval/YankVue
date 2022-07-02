<script setup>
defineProps({
  Link: {
    type: String,
    default: "#"
  }
})
</script>
<template>
  <a href="{{ Link }}"><slot></slot></a>
</template>

<style scoped>
  a {
    text-decoration: none;
    font-size: 20px;
    color: var(--primary);
    transition: 0.2s ease-out;
  }

  a:hover {
    color: var(--complementary);
    transition: 0.2s ease-in;
  }
</style>
