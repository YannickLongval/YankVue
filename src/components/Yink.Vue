<script setup>
defineProps({
  Link: {
    type: String,
    default: '#'
  }
})
</script>
<template>
  <a v-bind:href="Link"><slot></slot></a>
</template>

<style scoped>
  a {
    text-decoration: none;
    font-size: 20px;
    color: var(--primary);
    transition: all 0.2s ease-out;
  }

  a:hover {
    color: var(--complementary);
    transition: all 0.2s ease-in;
  }

  .dark{
    color: var(--background);
  }
</style>
