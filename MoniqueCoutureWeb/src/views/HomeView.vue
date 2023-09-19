<script setup lang="ts">
import MainGallery from '../components/MainGallery.vue';
import WelcomePage from '../components/WelcomePage.vue';
import HorizontalGallery from '../components/HorizontalGallery.vue';
</script>

<template>
  <main>
    <MainGallery />
    <WelcomePage />
    <HorizontalGallery gallery="Últimas creaciones" />
    <HorizontalGallery gallery="Tus favoritos" />
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  overflow: hidden;
  margin: 0;
  padding: 20px 80px;
  gap: 10px;
}
</style>
