<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import YankNavBar from './components/YankNavBar.vue'
import YankLink from './components/YankLink.vue'
import YankButton from './components/YankButton.vue'
import YankFooter from './components/YankFooter.vue'
</script>

<template>
 <YankNavBar NavTitle="HELLO">
  <YankLink Link="#about">About Me</YankLink>
  <YankLink Link="#Mission">Mission</YankLink>
  <YankLink Link="#Acheivements">What I do</YankLink>
  <YankButton>My Button</YankButton>
 </YankNavBar>
 
 <section>
    <img src="#" alt="YankLogo">
    <div class="text">
        <h1>HEY THERE!</h1>
        <p>In case you haven't noticed, this is a template website :P <br/>
        This is to show what features you can use and how to use the Yank components.</p>
    </div>
 </section>
 <YankFooter>
    <h1>HELLO</h1>
    <h2>World</h2>
 </YankFooter>
</template>

<style>
@import './assets/base.css';
@import './assets/bwpalette.css';

section {
    width: 80%;
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    height: 500px;
}
</style>
