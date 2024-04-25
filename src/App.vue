  <script setup>
  import Header from '@/components/Header.vue'
  import Body from '@/components/Body.vue'
  import Footer from '@/components/Footer.vue'
  import BudgetCalculation from '@/components/BudgetCalculation.vue'
</script>

<template>
  <v-app>
    <v-main>
      <v-container>
        <body> 

          <Header />
          <BudgetCalculation />
          
          <Body />
          <Footer />
          <router-view />
        </body>
      </v-container>
    </v-main>
  </v-app>
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