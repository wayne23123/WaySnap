<script setup>
import { useRoute } from 'vue-router';
import './assets/base.css';
import NavBar from './components/NavBar.vue';
import TheLayout from './components/TheLayout.vue';

const route = useRoute();
</script>

<template>
  <div v-if="route.name !== 'login'">
    <header class="header">
      <NavBar></NavBar>
    </header>

    <TheLayout>
      <router-view></router-view>
    </TheLayout>
  </div>

  <div v-else>
    <router-view></router-view>
  </div>
</template>

<style scoped>
.header {
  height: 80px;
  box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.8);
}
</style>
