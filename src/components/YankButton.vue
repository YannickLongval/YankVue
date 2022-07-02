<script setup>
</script>
<template>
  <button><slot></slot></button>
</template>

<style scoped>
    button {
        border: none;
        padding: 10px 20px;
        height: 50px;
        background-color: var(--complementary-light);
        font-size: 20px;
        color: var(--primary);
        border-radius: 10px;
        transition: 0.3s ease-out;
    }

    button:hover {
        cursor: pointer;
        background-color: var(--complementary-dark);
        color: var(--background);
        transition: 0.3 ease-in;
    }

</style>