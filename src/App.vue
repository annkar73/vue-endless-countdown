<script setup lang="ts">
import EndlessCounter from './components/EndlessCounter.vue';

</script>

<template>


  <main>
    <div id="app">
      <h1>Nedräkning till färdigt projekt</h1>
      <div class="counting">Det kommer vara klart om  <EndlessCounter />  sekunder!</div>
    </div>
  </main>
  
</template>

<style scoped>
h1 {
  font-size: 1.5em;
}

.counter {
  font-size: 1em;
}


</style>
