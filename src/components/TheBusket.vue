<template>
  <section class="busket">
    <div class="title-count">
      <h2 class="busket__title">Корзина</h2>
      <div class="busket__count">4</div>
    </div>
    <div class="busket__product">
      <img src="../assets/Rectangle 2.png" alt="" class="product__img" />
      <div class="product__info">
        <h4 class="info__title">Супер сырный</h4>
        <p class="info__weight">512г</p>
        <div class="info__price">550₽</div>
      </div>
      <div class="product__amount">
        <button class="minus" @click="count--">-</button>
        <div class="amount">{{ count }}</div>
        <button class="plus" @click="count++">+</button>
      </div>
    </div>
    <div class="busket__result-price">
      <p class="result-title">Итого</p>
      <div class="result-price">550₽</div>
    </div>
    <button class="submit__order">Оформить заказ</button>
    <div class="busket__delivery">
      <img src="../assets/delivery.svg" alt="" class="delivery__img" />
      <p class="delivery__price">Бесплатная доставка</p>
    </div>
  </section>
</template>

<script setup>
let count = 0;
</script>

<style scoped>
.busket {
  max-width: 300px;
  background-color: #fff;
  border-radius: 18px;
  margin-left: 75px;
  padding: 24px 16px 12px 24px;
}

.title-count {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #f2f2f3;
  padding-bottom: 12px;
}

.busket__title {
  font-size: 24px;
  font-weight: 600;
}

.busket__count {
  padding: 2px 16px;
  background-color: #f2f2f3;
  border-radius: 6px;
  font-size: 12px;
  line-height: 16px;
  letter-spacing: 0%;
  text-align: center;
}

.busket__product {
  display: flex;
  padding-top: 15px;
}

.product__img {
  max-width: 64px;
  height: 52px;
}

.product__info {
  font-size: 12px;
  margin-left: 6px;
}

.info__title {
}

.info__weight {
  color: rgb(177, 177, 177);
  padding: 1px 0 6px 0;
}

.info__price {
}

.product__amount {
  display: flex;
  align-items: center;
  background-color: #f2f2f3;
  border-radius: 12px;
  max-width: 84px;
  height: 40px;
  margin-left: 31px;
  border-bottom: 1px solid #f2f2f3;
}

.minus {
  border: none;
  padding-left: 9px;
}

.amount {
  font-size: 16px;
  padding: 9px 15px;
}

.plus {
  border: none;
  padding-right: 9px;
}

.busket__result-price {
  padding-top: 16px;
  padding-bottom: 24px;
  display: flex;
  justify-content: space-between;
  font-size: 16px;
}

.result-title {
}

.result-price {
}

.submit__order {
  border: none;
  background-color: #ff7020;
  padding: 12px 71px;
  border-radius: 12px;
  color: #fff;
  font-size: 15px;
}

.busket__delivery {
  font-size: 12px;
  display: flex;
  align-items: center;
  padding-top: 8px;
}

.delivery__img {
  margin-right: 8px;
}

.delivery__price {
}
</style>
