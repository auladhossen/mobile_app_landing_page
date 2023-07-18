<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Navbar from './components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import Features from './components/Features.vue'
import Team from './components/Team.vue'
import Contact from './components/Contact.vue'
import Pricing from './components/Pricing.vue'
</script>

<template>
  <Navbar></Navbar>
  <HeroSection></HeroSection>
  <Features></Features>
  <Pricing></Pricing>
  <Team></Team>
  <Contact></Contact>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
