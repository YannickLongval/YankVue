<script setup>
defineProps({
  NavTitle: {
    type: String,
    required: true
  }
})
</script>
<template>
<nav>
  <h1>{{ NavTitle }}</h1>
  <div id="navbar-items">
    <slot></slot>
  </div>
</nav>
</template>

<style scoped>
    
    * {
        background-color: var(--background-soft);

    }

    nav {
      width: 100%;
      height: 80px;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      padding: 0 40px;
    }

    h1{
      align-self: center;
      font-size: 30px;
    }

    #navbar-items{
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
      width: 500px;
    }
</style>
