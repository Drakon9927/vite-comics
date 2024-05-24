<script setup>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>



<style scoped>
#app {
    display: flex;
    flex-direction: column;

}
</style>
