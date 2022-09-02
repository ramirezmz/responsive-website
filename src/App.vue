<template>
  <body>
    <NavBar />
    <HeroSection />
    <AboutSection />
  </body>
</template>
<script setup lang="ts">
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import AboutSection from './components/AboutSection.vue'

</script>
<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Kumbh Sans', sans-serif;
  scroll-behavior: smooth;
}
</style>
