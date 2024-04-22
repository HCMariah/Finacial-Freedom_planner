<script setup="ts">
import Header from './components/Header.vue'
import Body from './components/Body.vue'
import footer from './components/footer.vue'
</script>

<template>
  <div class="container">

    <Header />

    <Body />

    <footer />
  </div>
</template>

<style>
.container {
  border: solid;
  width: 100%;
  padding-right: 2rem;
  padding-left: 2rem;
  padding-bottom: 2rem;
  position: relative;
}
</style>
