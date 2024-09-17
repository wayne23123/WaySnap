<script setup>
import './assets/base.css';
import NavBar from './components/NavBar.vue';
</script>

<template>
  <header class="header">
    <NavBar></NavBar>
  </header>

  <router-view></router-view>
</template>

<style scoped>
.header {
  height: 80px;
  box-shadow: 0px 4px 24px rbga(0, 0, 0, 0.8);
}
</style>
