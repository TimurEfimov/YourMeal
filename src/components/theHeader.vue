<template>
    <header class="header__container">
      <div class="logo">
        <a href="#" class="logo__text">YourMeal</a>
        <img src="../assets/logo.png" alt="" class="logo__png" />
      </div>
      <div class="welcome__text">
        <img src="../assets/pic.png" alt="" />
        <div class="welcome__intext">
          <h1 class="welcome__title">
            Только самые <span>сочные бургеры!</span>
          </h1>
          <p class="welcome__delivery">Бесплатная доставка от 599₽</p>
        </div>  
      </div>
    </header>
</template>

<script>
export default {};
</script>

<style scoped>
/* Start logo */
.header__container {
  background-image: url("./../assets/bg.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
}

.header__container {
  display: flex;
  flex-direction: column;
  align-items: center;
  /* max-width: 785px;
  margin: 0 auto; */
}

.logo {
  display: flex;
  align-items: center;
  padding: 22px 315px;
}

.logo__text {
  color: #fff;
  font-weight: 700;
  font-size: 24px;
}

.logo__png {
  padding-left: 4px;
}
/* Finish logo */

/* Start welcome */
.welcome__text {
  display: flex;
  padding-bottom: 63px;
}

.welcome__title {
  font-size: 50px;
  font-weight: 800;
  color: #fff;
  line-height: 120%;
  display: flex;
  flex-direction: column;
}
span {
  color: #ff5c00;
}

.welcome__intext {
  margin-left: 21px;
  padding-top: 46px;
}

.welcome__delivery {
  color: #fff;
  margin-top: 52px;
  font-size: 16px;
}
/* Finish welcome */
</style>
