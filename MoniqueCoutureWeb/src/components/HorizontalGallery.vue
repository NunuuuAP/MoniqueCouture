<script setup lang="ts">
    defineProps<{
      gallery: string
      elements: number
    }>()

</script>

<template>
  <section>
    <h2 id="title">{{ gallery }}</h2>
    <div class="gallery">
      <div class="element" v-for="index in elements" :key="index">
        <img src="./assets/bolso.jpeg" alt="Creation 1" />
        <div id="productName">Nombre del producto</div>
        <div id="productPrice">Precio X€</div>
      </div>
    </div>
  </section>
</template>
  
<style scoped>
section {
  margin: 20px 0;
}

#title {
  font-weight: 500;
  font-size: 2em;
  text-align: center;
}
.gallery {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
  max-width: 100%;
  gap: 10px;
  
}
.element {
  display: flex;
  flex-direction: column;
  flex: 0 0 calc(25% - 15px);
  margin: 15px 0;
}
.element img {
  width: 100%;
  height: fit-content;
  aspect-ratio: 3/4;
  margin-bottom: 20px;
}

#productPrice, #productName {
  text-align: center;
}

#productName {
  color: var(--accent);
  font-weight: bold;
}

#productPrice {
  color: var(--typo);
}
</style>