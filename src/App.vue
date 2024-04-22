<script setup="ts">
import Header from './components/Header.vue'
import Body from './components/Body.vue'
import Footer from './components/footer.vue'
import CalculationFunction from './components/CalculationFunction.vue';
</script>

<template>
  <div class="container">

    <Header />

    <Body />

    <CalculationFunction />

    <Footer />

  </div>
</template>

<style>
.container {
  width: 100%;
  padding-right: 2rem;
  padding-left: 2rem;
  padding-bottom: 2rem;
  text-align: center;
}
</style>
