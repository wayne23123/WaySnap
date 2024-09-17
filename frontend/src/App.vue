<script setup>
import './assets/base.css';
import NavBar from './components/NavBar.vue';
import TheLayout from './components/TheLayout.vue';
</script>

<template>
  <header class="header">
    <NavBar></NavBar>
  </header>

  <TheLayout>
    <router-view></router-view>
  </TheLayout>
</template>

<style scoped>
.header {
  height: 80px;
  box-shadow: 0px 4px 24px rbga(0, 0, 0, 0.8);
}
</style>
