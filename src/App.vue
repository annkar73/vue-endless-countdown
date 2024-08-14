<script setup lang="ts">
import EndlessCounter from './components/EndlessCounter.vue';
</script>

<template>
  <main>
    <div id="app">
      <h1>Nedräkning till färdigt projekt</h1>
      <div class="countdown-container">
        <p>Det kommer vara klart om</p>
        <div class="counter">
          <EndlessCounter />
        </div>
        <p>sekunder. Jag lovar!!</p>
      </div>
    </div>
  </main>
</template>

<style scoped>

main {
  display: flex;
  justify-content: center;
  align-items: center; 
  height: 100vh; 
  margin: 0; 
  background-color: #f0f0f0; 
}

#app {
  text-align: center; 
}

h1 {
  font-size: 2em; 
  font-weight: bold;
  margin-bottom: 0.5em; 
}

.countdown-container {
  display: flex;
  flex-direction: column; 
  align-items: center; 
  gap: 0.5em; 
}

.counter {
  font-size: 2em; 
  font-weight: bold;
  margin: 0.5em 0; 
}

p {
  font-size: 1.5em; 
  margin: 0; 
}
</style>
