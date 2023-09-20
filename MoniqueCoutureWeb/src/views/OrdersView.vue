<script setup lang="ts">
import HorizontalGallery from '../components/HorizontalGallery.vue';
</script>

<template>
    <div class="orders">
      <hr><h1>POR ENCARGO</h1><hr>
      <HorizontalGallery gallery="" :elements="20"/>
    </div>
</template>

<style>
.orders {
  min-height: 40vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0 5px;
}

hr {
  border-color: var(--accent-typo);
  border-style: solid;
  border-width: 0.001pt;
  width: 100%;
}
</style>