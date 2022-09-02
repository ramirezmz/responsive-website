<template>
  <div class="hero" id="home">
    <div class="hero__container">
      <h1 class="hero__heading">Choose your <span>colors</span></h1>
      <p class="hero__description">Unlimited Possibilities</p>
      <button class="main__btn"><a href="#">Explore</a></button>
    </div>
  </div>
</template>
<style>
.hero {
  background: #000000;
  background: linear-gradient(to right, #161616, #000000);
  padding: 200px 0;
}

.hero__container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  height: 90%;
  text-align: center;
  padding: 30px;
}

.hero__heading {
  font-size: 100px;
  margin-bottom: 24px;
  color: #fff;
}

.hero__heading span {
  background: #ee0979;
  background: -webkit-linear-gradient(to right, #ff6a00, #ee0979);
  background: linear-gradient(to right, #ff6a00, #ee0979);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
.hero__description {
  font-size: 60px;
  background: #da22ff;
  background: -webkit-linear-gradient(to right, #9114ff, #da22ff);
  background: linear-gradient(to right, #8f0eff, #da22ff);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

.highlight {
  border-bottom: 4px solid rgb(132, 0, 255);
}

@media screen and (max-width: 768px) {
  .hero__heading {
    font-size: 60px;
  }

  .heading__description {
    font-size: 40px;
  }
}
</style>