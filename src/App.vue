<script setup lang="ts">
import EndlessCounter from './components/EndlessCounter.vue';

</script>

<template>


  <main>
    <div id="app">
      <h1>Nedräkning till färdigt projekt</h1>
      <h2>Det kommer vara klart om  <EndlessCounter />  sekunder!</h2>
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

h2 {
  font-size: 1.5em;
}

#app > h2 {
  margin-top: 0;
}

</style>
