<script setup>
</script>
<template>
  <section>
    <slot></slot>
  </section>
</template>

<style scoped>
  section {
    width: 80%;
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    height: 550px;
    background-color: var(--background);
    padding-top: 100px;
  }
</style>