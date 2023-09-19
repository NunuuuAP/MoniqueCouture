<script setup lang="ts">
import HeaderBanner from '../components/HeaderBanner.vue';
import HeaderMenu from '../components/HeaderMenu.vue';
import MainGallery from '../components/MainGallery.vue';
import PageFooter from '../components/PageFooter.vue';
import WelcomePage from '../components/WelcomePage.vue';
import HorizontalGallery from '../components/HorizontalGallery.vue';
</script>

<template>
  <main>
    <div id="webpagecontent">
        <MainGallery />
        <WelcomePage />
        <HorizontalGallery gallery="Últimas creaciones" />
        <HorizontalGallery gallery="Los favoritos" />
    </div>
  </main>
</template>

<style scoped>
#webpagecontent {
  display: block;
  overflow: hidden;
  margin: 0;
  padding: 20px 80px;
}
</style>
