<template>
  <nav class="navbar">
    <div class="navbar__container">
      <a href="#home" id="navbar__logo">COLOR</a>
      <div class="navbar__toggle" id="mobile-menu">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
      <ul class="navbar__menu">
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
<script lang="ts">
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
  background-color: #f81777;
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

</style>