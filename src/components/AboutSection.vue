<template>
  <div class="main" id="about">
    <div class="main__container">
      <div class="main__img__container">
        <div class="main__img__card">ICON</div>
      </div>
      <div class="main__content">
        <h1>What do we do?</h1>
        <h2>We help bussinesses scale</h2>
        <p>Schedule a call to learn more about our services</p>
        <button class="main__btn"><a href="#">Schedule Call</a></button>
      </div>
    </div>
  </div>
</template>
<style>
.main {
  background-color: #131313;
  padding: 10rem 0;
}

.main__container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-content: center;
  margin: 0 auto;
  height: 90%;
  z-index: 1;
  width: 100%;
  max-width: 1300px;
  padding: 0 50px;
}

.main__content {
  color: #fff;
  width: 100%;
}

.main__content h1 {
  font-size: 2rem;
  background-color: #fe3b6f;
  background-image: linear-gradient(to top, #ff087b 0%, #ed1a52 100%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
  text-transform: uppercase;
  margin-bottom: 32px;
}

.main__content h2 {
  font-size: 4rem;
  background: #ff8177;
  background: -webkit-linear-gradient(to right, #9114ff, #da22ff);
  background: linear-gradient(to right, #8f0eff, #da22ff);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

.main__content p {
  margin: 1rem;
  font-size: 2rem;
  font-weight: 700;
}

.main__btn {
  font-size: 1.8rem;
  background: #833ab4;
  background: -webkit-linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
  background: linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
  padding: 20px 60px;
  border: none;
  border-radius: 4px;
  margin-top: 2rem;
  cursor: pointer;
  position: relative;
  transition: all 0.35s;
  outline: none;
}

.main__btn a {
  position: relative;
  z-index: 2;
  color: #fff;
  text-decoration: none;
}

.main__btn:after {
  position: absolute;
  content: '';
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: #ff1ead;
  transition: all 0.35s;
  border-radius: 4px;
}

.main__btn:hover {
  color: #fff;
}

.main__btn:hover:after {
  width: 100%;
}

.main__img__container {
  text-align: center;
}

.main__img__card {
  margin: 10px;
  height: 500px;
  width: 500px;
  border-radius: 4px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: #fff;
  background-image: linear-gradient(to right, #00dbde 0%, #fc00ff 100%);
}

/*Mobile Responsive */
@media screen and (max-width: 1100px) {
  .main__container {
    display: grid;
    grid-template-columns: 1fr;
    align-items: center;
    justify-content: center;
    width: 100%;
    margin: 0 auto;
    height: 90%;
  }

  .main__img__container {
    display: flex;
    justify-content: center;
  }

  .main__img__card {
    height: 425px;
    width: 425px;
  }

  .main__content {
    text-align: center;
    margin-bottom: 4rem;
  }

  .main__content h1 {
    font-size: 2.5rem;
    margin-top: 2rem;
  }

  .main__content p {
    margin-top: 1rem;
    font-size: 1.5rem;
  }
}

@media screen and(max-width: 480px) {
  .main__img__card {
    width: 250px;
    height: 250px;
  }

  .main__content h1 {
    font-size: 2rem;
    margin-top: 3rem;
  }

  .main__content h2 {
    font-size: 2rem;
  }

  .main__content p {
    margin-top: 2rem;
  }

  .main__btn {
    padding: 12px 36px;
    margin: 2.5rem 0;
  }
}

</style>