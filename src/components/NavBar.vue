<template>
  <nav class="navbar">
    <div class="navbar__container">
      <a href="#home" id="navbar__logo">COLOR</a>
      <div  @click="mobileMenu" class="navbar__toggle" :class="{ active: isX }" id="mobile-menu">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
      <ul class="navbar__menu" :class="{ active: isActive}">
        <li class="navbar__item">
          <a href="#home" class="navbar__links" id="home-page">Home</a>
        </li>
        <li class="navbar__item">
          <a href="#about" class="navbar__links" id="about-page">About</a>
        </li>
        <li class="navbar__item">
          <a href="#services" class="navbar__links" id="home-page">Services</a>
        </li>
        <li class="navbar__btn">
          <a href="#sign-up" class="button" id="signup">Sign Up</a>
        </li>
      </ul>
    </div>
  </nav>
</template>
<script setup lang="ts">
import { ref } from 'vue'

const isX = ref(false)
const isActive = ref(false)

const mobileMenu = () => {
  isActive.value = !isActive.value
  isX.value = !isX.value
}

</script>
<style scoped>
.navbar {
  background: #131313;
  height: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.2rem;
  position: sticky;
  top: 0;
  z-index: 999;
}

.navbar__container {
  display: flex;
  justify-content: space-between;
  height: 80px;
  z-index: 1;
  width: 100%;
  max-width: 1300px;
  margin: 0 auto;
  padding: 0 50px;
}

#navbar__logo {
  background-color: #ff8177;
  background-image: linear-gradient(to top, #ff0844 0%, #ffb199 100%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
  display: flex;
  align-items: center;
  cursor: pointer;
  text-decoration: none;
  font-size: 2rem;
}

.navbar__menu {
  display: flex;
  align-items: center;
  list-style: none;
}

.navbar__item {
  height: 80px;
}

.navbar__links {
  color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 125px;
  text-decoration: none;
  height: 100%;
  transition: all 0.3s ease;
}

.navbar__btn {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 1rem;
  width: 100%;
}

.button {
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  padding: 10px 20px;
  height: 100%;
  width: 100%;
  border: none;
  outline: none;
  border-radius: 4px;
  background: #833ab4;
  background: -webkit-linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
  background: linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
  color: #fff;
  transition: all 0.3s ease;
}

.navbar__links:hover {
  color:#9518fc;
  transition: all 0.3s ease;
}

@media screen and (max-width: 960px) {
  .navbar__container {
    display: flex;
    justify-content: space-between;
    height: 80px;
    z-index: 1;
    width: 100%;
    max-width: 1300px;
    padding: 0;
  }
  .navbar__menu {
    display: grid;
    grid-template-columns: auto;
    margin: 0;
    width: 100%;
    position: absolute;
    top: -1000px;
    opacity: 1;
    transition: all 0.5s ease;
    z-index: -1;
  }

  .navbar__menu.active {
    background: #131313;
    top: 100%;
    opacity: 1;
    transition: all 0.5s ease;
    z-index: 99;
    height: 60hv;
    font-size: 1.6rem;
  }

  #navbar__logo {
    padding-left: 25px;
  }
  .navbar__toggle .bar {
    width: 25px;
    height: 3px;
    margin: 5px auto;
    transition: all 0.3s ease-in-out;
    background: #fff;
  }
  .navbar__item {
    width: 100%;
  }
  .navbar__links {
    text-align: center;
    padding: 2rem;
    width: 100%;
    display: table;
  }

  .navbar__btn {
    padding-bottom: 2rem;
  }

  .button {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 80%;
    height: 80px;
    margin: 0;
  }

  #mobile-menu {
    position: absolute;
    top: 20%;
    right: 5%;
    transform: translate(5%, 20%);  
  }
  .navbar__toggle .bar {
    display: block;
    cursor: pointer;
  }

  #mobile-menu.active .bar:nth-child(2) {
    opacity: 0;
  }

  #mobile-menu.active .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
  }

  #mobile-menu.active .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
  }
}
</style>