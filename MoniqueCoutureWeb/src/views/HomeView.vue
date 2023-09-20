<script setup lang="ts">
import MainGallery from '../components/MainGallery.vue';
import WelcomePage from '../components/WelcomePage.vue';
import HorizontalGallery from '../components/HorizontalGallery.vue';
</script>

<template>
  <main>
    <MainGallery />
    <WelcomePage />
  </main>
  <section>
    <HorizontalGallery gallery="Últimas creaciones" :elements="4"/>
    <HorizontalGallery gallery="Tus favoritos" :elements="4"/>
  </section>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  overflow: hidden;
  margin: 0;
  padding: 0 80px;
  gap: 10px;
}

section {
  display: flex;
  flex-direction: column;
  overflow: hidden;
  padding: 0 5px;
  gap: 10px;
}
</style>
