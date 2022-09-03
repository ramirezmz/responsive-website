<template>
  <div class="services" id="services">
    <h1>Our services</h1>
    <div class="services__wrapper">
      <div class="services__card">
        <h2>Custom Colorways</h2>
        <p>AI Powered technology</p>
        <div class="services__btn"><button>Get started</button></div>
      </div>
      <div class="services__card">
        <h2>Are you ready?</h2>
        <p>Tech the lepa</p>
        <div class="services__btn"><button>Get started</button></div>
      </div>
      <div class="services__card">
        <h2>Full Gradients</h2>
        <p>100 Combinations</p>
        <div class="services__btn"><button>Get started</button></div>
      </div>
      <div class="services__card">
        <h2>Infinity Choises</h2>
        <p>1000's of colors</p>
        <div class="services__btn"><button>Get started</button></div>
      </div>
    </div>
  </div>
</template>
<style>
.services {
  background: #131313;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  padding: 10rem 0;
}

.services h1 {
  background-color: #ff8177;
  background-image: linear-gradient(to right, #ff0844 0%, #f7673c 100%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
  margin-bottom: 5rem;
  font-size: 2.5rem;
}

.services__wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-row: 1fr;
}

.services__card {
  margin: 10px;
  height: 425px;
  width: 300px;
  border-radius: 4px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: #fff;
  background-image: linear-gradient(to right, #00dbde 0%, #fc00ff 100%);
  transition: 0.3s ease-in;
}

.services__card:nth-child(2) {
  background: #24C6DC;
  background: -webkit-linear-gradient(to right, #514A9D, #24C6DC);
  background: linear-gradient(to right, #514A9D, #24C6DC);
}
.services__card:nth-child(3) {
  background: #4776E6;
  background: -webkit-linear-gradient(to right, #8E54E9, #4776E6);
  background: linear-gradient(to right, #8E54E9, #4776E6);
}

.services__card:nth-child(4) {
  background: #FF8008;
  background: -webkit-linear-gradient(to right, #FFC837, #FF8008);
  background: linear-gradient(to right, #FFC837, #FF8008);
}

.services__card h2 {
  text-align: center;
}

.services__card p {
  text-align: center;
  margin-top: 24px;
  font-size: 20px;
}

.services__btn {
  display: flex;
  justify-content: center;
  margin-top: 16px;
}

.services__card button {
  color: #fff;
  padding: 14px 24px;
  border: none;
  outline: none;
  border-radius: 4px;
  background: #131313;
  font-size: 1rem;
}

.services__card button:hover {
  cursor: pointer;
}
.services__card:hover {
  transform: scale(1.075);
  transition: 0.3s ease-in;
  cursor: pointer;
}

@media screen and (max-width: 1300px) {
  .services__wrapper {
    grid-template-columns: 1fr 1fr;
  }
}

@media screen and (max-width: 768px) {
  .services__wrapper {
    grid-template-columns: 1fr;
  }
}

</style>