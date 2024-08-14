<script setup lang="ts">

import { ref, onMounted, onBeforeUnmount } from 'vue';

const countdown = ref(getRandomNumber()); // Initialiserar med ett slumpmässigt värde
const minStartValue = 12;
const maxStartValue = 100;
const minRandomValue = 3;
const maxRandomValue = 15;

let intervalId: ReturnType<typeof setInterval> | undefined;

function getRandomNumber() {
  return Math.floor(Math.random() * (maxStartValue - minStartValue + 1)) + minStartValue;
}
function getRandomMinValue() {
  return Math.floor(Math.random() * (maxRandomValue - minRandomValue +1)) + minRandomValue;
}

function startCountdown() {
  const minValue = getRandomMinValue();
  
  intervalId = setInterval(() => {
    if (countdown.value > minValue) {
      countdown.value--;

    } else {
      countdown.value = getRandomNumber();


    }
  }, 1000);
}


onMounted(() => {
  startCountdown();
});

onBeforeUnmount(() => {
  clearInterval(intervalId);
})
</script>

<template>
    <span class="counter">{{  countdown }}</span>
</template>


<style scoped>
.counter {
  color: red;
  font-size: 2.5em;
  font-weight: bold;
}

</style>