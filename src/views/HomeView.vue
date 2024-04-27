<script>
import Header from '@/components/Header.vue';
import BudgetCalculation from '@/components/BudgetCalculation.vue';
import Body from '@/components/Body.vue';
import Bottom from '@/components/Bottom.vue';
</script>

<template>
  <title>Financial Freedom</title>
  <div class="container">
    <Header />
    <BudgetCalculation />
    <Body />
    <Bottom />
  </div>
</template>

<style>
.container {
  width: 100%;
  padding-right: 2rem;
  padding-left: 2rem;
  padding-bottom: 1rem;
  text-align: center;
  text-wrap:balance;
}
a {
  text-decoration: none;
  color: #0CBD6E;
}
</style>