<template>
  <nav>
    <ul>
      <li v-for="(item, i) in navigation" :key="i">
        <img :src="item.url" alt="logo" />
        <a>{{ item.name }}</a>
      </li>
    </ul>
  </nav>
</template>

<script setup>
import cheeseburger from "../assets/navIcons/cheeseburger.svg";
import onion from "../assets/navIcons/onion.svg";
import hotdog from "../assets/navIcons/hotdog.svg";
import donat from "../assets/navIcons/donat.svg";
import fastFood from "../assets/navIcons/fast-food.svg";
import pizza from "../assets/navIcons/pizza.svg";
import saus from "../assets/navIcons/saus.svg";
import shaurma from "../assets/navIcons/shaurma.svg";
import wok from "../assets/navIcons/wok.svg";

let navigation = [
  {
    name: "Бургеры",
    url: cheeseburger,
  },
  {
    name: "Закуски",
    url: onion,
  },
  {
    name: "Хот-доги",
    url: hotdog,
  },
  {
    name: "Комбо",
    url: fastFood,
  },
  {
    name: "Шаурма",
    url: shaurma,
  },
  {
    name: "Пицца",
    url: pizza,
  },
  {
    name: "Вок",
    url: wok,
  },
  {
    name: "Десерты",
    url: donat,
  },
  {
    name: "Соусы",
    url: saus,
  },
];
</script>

<style scoped>
nav {
  margin-left: 50px;
  margin-right: 50px;
  margin-top: 40px;
}
ul {
  display: flex;
  overflow-x: scroll;
  justify-content: space-around;
}
li {
  display: flex;
  align-items: center;
  padding: 9px 14px;
  background-color: #fff;
  border-radius: 50px;
  transition: 0.3s;
  border: solid 1px #fff;
}
img {
  margin-right: 8px;
}

li:hover {
  border: solid 1px #F86310;
}

</style>
