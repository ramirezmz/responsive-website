<template>
  <body>
    <NavBar />
    <HeroSection />
    <AboutSection />
    <Services />
    <Feature />
    <Footer />
  </body>
</template>
<script setup lang="ts">
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import AboutSection from './components/AboutSection.vue'
import Services from './components/Services.vue';
import Feature from './components/Feature.vue';
import Footer from './components/Footer.vue';

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
