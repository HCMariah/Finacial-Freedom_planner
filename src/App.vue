<script setup="ts">
import Header from './components/Header.vue'
import Body from './components/Body.vue'
import Footer from './components/footer.vue'
import Calculation from './components/Calculation.vue';
</script>

<template>
  <v-container>

    <Header />

    <Body />

    <Calculation />

    <Footer />

  </v-container>
</template>

<style>
.container {
  width: 100%;
  padding-right: 1rem;
  padding-left: 1rem;
  padding-bottom: 1rem;
  text-align: center;
}
</style>
