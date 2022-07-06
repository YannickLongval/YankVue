<script setup>
defineProps({
  NavTitle: {
    type: String,
    default: ''
  },
  NavLogo: {
    type: String,
    default: ''
  }
})
</script>
<template>
<nav>
  <img v-if="NavLogo != ''" v-bind:src="'./src/components/icons/' + NavLogo" alt="LOGO"/>
  <h1 v-if="NavTitle != ''">{{NavTitle}}</h1>
  <div id="navbar-items">
    <slot></slot>
  </div>
</nav>
</template>

<style scoped>

    nav {
      position: sticky;
      z-index: 100;
      top: 0;
      width: 100%;
      height: 80px;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      padding: 0 40px;
      background-color: var(--background-soft);
    }

    img {
      height: 60px;
      margin: auto 0;
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
    .dark{
      background-color: var(--primary-soft);
    }

</style>
