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
  padding-right: 5rem;
  padding-left: 5rem;
  padding-bottom: 1rem;
  text-align: center;
}
a {
  text-decoration: none;
  color: #0CBD6E;
}
</style>