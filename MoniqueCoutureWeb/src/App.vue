<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HeaderBanner from './components/HeaderBanner.vue';
import PageFooter from './components/PageFooter.vue';
</script>

<template>
  <HeaderBanner />
  <header>
    <div class="background">
      <img src="../assets/logo.png" alt="Monique Couture logo" />
      <nav>
        <RouterLink to="/">Inicio</RouterLink>
        <RouterLink to="/orders">Encargos</RouterLink>
        <RouterLink to="/fabrics">Tejidos</RouterLink>
        <RouterLink to="/about">Sobre nosotros</RouterLink>
        <RouterLink to="/account">Mi cuenta</RouterLink>
        <!--<input v-model="search">-->
      </nav>
    </div>
  </header>
  <RouterView />
  <PageFooter />
</template>

<style scoped>

header .background {
  position: sticky;
  top: 0;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  background-color: var(--background);
  color: var(--typo);
  width: 100vw;
  height: fit-content;
  padding: 50px 0 30px 0;
  text-align: center;
}

nav {
  display: flex;
  gap: 50px;
}

</style>
