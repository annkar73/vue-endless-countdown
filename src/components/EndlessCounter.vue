<script setup lang="ts">

import { ref, onMounted, onBeforeUnmount } from 'vue';

const countdown = ref(getRandomNumber());
let intervalId: ReturnType<typeof setInterval> | undefined;

function getRandomNumber() {
  return Math.floor(Math.random() *96) + 5;
}

function startCountdown() {
  intervalId = setInterval(() => {
    if (countdown.value <= 3) {
      countdown.value = getRandomNumber();

    } else {
      countdown.value--;

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