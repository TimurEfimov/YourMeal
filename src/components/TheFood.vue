<template>
  <main class="main">
    <h2 class="main__title">Бургеры</h2>
    <div class="main__card">
      <a href="#" class="info__card" v-for="(item, i) in cards" :key="i">
        <img :src="item.url" alt="" class="info__img" />
        <div class="info__price">{{ item.price }}₽</div>
        <h5 class="info__title">{{ item.name }}</h5>
        <div class="info__weight">{{ item.weight }}г</div>
        <button class="info__enterBusket">Добавить</button>
      </a>
    </div>
  </main>
</template>

<script setup>
import classic from "../assets/foodCards/alwaysClassic.png";
import full from "../assets/foodCards/full.png";
import blow from "../assets/foodCards/heavyBlow.png";
import italic from "../assets/foodCards/italic.png";
import meetbomb from "../assets/foodCards/meetBomb.png";
import cheezy from "../assets/foodCards/veryCheezy.png";

let cards = [
  {
    url: meetbomb,
    price: 689,
    name: "Мясная бомба",
    weight: 520,
  },
  {
    url: cheezy,
    price: 550,
    name: "Супер сырный",
    weight: 512,
  },
  {
    url: full,
    price: 639,
    name: "Сытный",
    weight: 580,
  },
  {
    url: blow,
    price: 480,
    name: "Тяжелый удар",
    weight: 470,
  },
  {
    url: classic,
    price: 450,
    name: "Вечная классика",
    weight: 450,
  },
  {
    url: meetbomb,
    price: 689,
    name: "Мясная бомба",
    weight: 520,
  },
  {
    url: italic,
    price: 560,
    name: "Итальянский",
    weight: 510,
  },
];
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  padding-bottom: 100px;
}

.main__title {
  font-size: 40px;
  font-weight: 600;
  padding-bottom: 24px;
}

.main__card {
  background-color: #fff;
  max-width: 300px;
  border-radius: 18px;
  padding: 12px;
  margin: 0 30px 30px 30px;
}

.info__card {
  color: #000000;
  font-size: 16px;
}

.info__img {
  max-width: 276px;
  height: 220px;
}

.info__price {
  padding: 16px 0 8px 0;
  font-size: 24px;
  font-weight: 600;
}

.info__title {
}

.info__weight {
  color: rgb(177, 177, 177);
  padding: 29px 0 8px 0;
}

.info__enterBusket {
  border-radius: 12px;
  background: rgb(242, 242, 243);
  text-align: center;
  padding: 12px 102px;
  transition: 0.3s;
}

.info__enterBusket:hover {
  background-color: #ffab08;
  color: #fff;
}
</style>
