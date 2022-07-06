<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import YavBar from './components/YavBar.vue'
import Yink from './components/Yink.vue'
import Yutton from './components/Yutton.vue'
import Yooter from './components/Yooter.vue'
import Yection from './components/Yection.vue'
</script>

<template>
 <YavBar NavLogo="YankLogoW.png" class='dark'>
  <Yink Link='#Section1' class="dark">Section 1</Yink>
  <Yink Link='#Section2' class="dark">Section 2</Yink>
  <Yink Link="#Section3" class="dark">Section 3</Yink>
  <Yutton @click="clickMe()">My Button</Yutton>
 </YavBar>
 
 <Yection id="Section1">
    <img src="./components/icons/YankLogo.png" alt="YankLogo" style="width: 400px;"/>
    <div class="text">
        <h2>Section 1</h2>
        <p>This is where you introduce the purpose of the website. In this case, we are showcasing the Yank.vue capabilities.</p>
    </div>
 </Yection>
 <Yection id="Section2">
    <div class="text">
        <h2>Section 2</h2>
        <p>Now that your audience knows the purpose of the website, this is when you get more into detail about the purpose and why they should care. Something along the lines of...</p>
    </div>
    <div class="text">
        <h3>“With Yank.vue, you can <i>accelerate</i> your web development for <i>maximum</i> efficiency. Use the Yomponents (Yank components) to <i>easily</i> build your website”</h3>
    </div>
 </Yection>

 <Yection id="Section3">
    <div class="text full">
        <h1>Section 3</h1>
        <p>This is where you put your call to action. What do you want your audience to do? It could just be for awareness and you could include a button to promote something (just like this button that brring yout to the github for Yank.vue, which you should check out).</p>
        <Yutton @click="newTab('https://github.com/YannickLongval/YankVue')">Try out Yank.vue</Yutton>
    </div>
 </Yection>

 <Yooter>
    <div class="contact">
        <h1>Contact</h1>
        <Yink Link="https://github.com/YannickLongval" target="_blank" class="dark">github</Yink>
    </div>
    
 </Yooter>
</template>

<script>
    function clickMe() {
        alert("I don't actually do anything :P")
    }

    function newTab(url) {
        window.open(url)
    }
</script>

<style>
@import './assets/base.css';
@import './assets/bwpalette.css';

.text {
    color: var(--primary);
    width: 400px;
}

.text.full {
    width: 800px;
    text-align: center;
}

.text h1{
    font-size: 80px;
}

.text h2{
    font-size: 60px;
}

.text h3{
    font-size: 30px;
}
.text p{
    font-size: 20px;
    margin-bottom: 20px;
}

html{
    scroll-behavior: smooth;
}
</style>
