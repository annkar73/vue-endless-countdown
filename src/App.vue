<script setup lang="ts">
import EndlessCounter from './components/EndlessCounter.vue';
</script>

<template>
  <main>
    <div id="app">
      <h1>Snart är det klart!</h1>
      <div class="countdown-container">
        <p>Det är bara</p>
        <div class="counter">
          <EndlessCounter />
        </div>
        <p>sekunder kvar.</p> 
        <h3>Jag lovar!!</h3>
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
  margin: none; 
  padding: none;
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
h3 {
  padding: 10px 50px;
  color: red;
  font-weight: bolder;
  font-size: 1.7em;
  text-transform: uppercase;
}
</style>
