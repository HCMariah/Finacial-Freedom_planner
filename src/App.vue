<script setup="ts">
import Header from './components/Header.vue'
import Body from './components/Body.vue'
</script>

<template>
  <div class="container">
    <Header />

    <Body />
  </div>
</template>

<style>
.container {
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  padding-right: 2rem;
  padding-left: 2rem;
  position: relative;
}
</style>
