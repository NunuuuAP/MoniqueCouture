<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HeaderBanner from './components/HeaderBanner.vue';
import PageFooter from './components/PageFooter.vue';
</script>

<template>
  <HeaderBanner />
    <div id="header">
      <img src="./assets/LogoPruebas.svg" alt="Monique Couture logo" />
      <nav>
        <RouterLink to="/">Inicio</RouterLink>
        <RouterLink to="/orders">Por encargo</RouterLink>
        <RouterLink to="/fabrics">Tejidos</RouterLink>
        <RouterLink to="/about">Sobre nosotros</RouterLink>
        <RouterLink to="/account">Mi cuenta</RouterLink>
        <!--<input v-model="search">-->
      </nav>
    </div>
  <RouterView />
  <PageFooter />
</template>

<style scoped>

#header {
  position: sticky;
  top: 0;
  display: flex;
  flex: 1;
  flex-direction: row;
  justify-content: space-between;
  align-items: flex-end;
  background-color: var(--background);
  color: var(--typo);
  width: 100vw;
  height: fit-content;
  padding: 15px 85px 10px 85px;
  text-align: center;
  gap: 20px;
}

nav {
  display: flex;
  justify-content: flex-end;
  flex: 1;
  gap: 40px;
}

nav a {
  text-decoration: none;
  color: var(--typo);
  font-size: 1.2em;
}

#header img {
  width: 15%;
  min-width: 80px;
}

</style>
