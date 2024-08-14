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
h1 {
  font-size: 1.5em;
  font-weight: bold;
}

h2 {
  font-size: 1em;
}


</style>
