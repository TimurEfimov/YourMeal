<template>
  <div>
    <theHeader />
    <theNavigation />
    <div class="main__things">
      <theBusket />
      <theFood />
    </div>
  </div>
</template>

<script setup>
import theHeader from "./components/theHeader.vue";
import theNavigation from "./components/TheNavigation.vue";
import theBusket from "./components/TheBusket.vue";
import TheFood from "./components/TheFood.vue";
</script>

<style>
.main__things {
  display: flex;
}
</style>
