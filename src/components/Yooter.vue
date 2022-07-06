<script setup>
</script>
<template>
  <footer>
    <div id="footer-items">
        <slot></slot>
    </div>
  </footer>
</template>

<style scoped>
    footer {
        width: 100%;
        height: 200px;
        margin-top: auto;
        background-color: var(--primary-soft);
        color: var(--background);
        padding: 20px 100px;
    }

    #footer-items{
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
      width: 500px;
    }

</style>