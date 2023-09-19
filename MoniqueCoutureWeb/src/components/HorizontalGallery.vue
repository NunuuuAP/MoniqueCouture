<script setup lang="ts">
    defineProps<{
      gallery: string
    }>()
</script>

<template>
  <section>
    <h2 id="title">{{ gallery }}</h2>
    <div class="gallery">
      <div class="element">
        <img src="./assets/bolso.jpeg" alt="Creation 1" />
        <div id="productName">Nombre del producto</div>
        <div id="productPrice">Precio X€</div>
      </div>
      <div class="element">
        <img src="./assets/bolso.jpeg" alt="Creation 1" />
        <div id="productName">Nombre del producto</div>
        <div id="productPrice">Precio X€</div>
      </div>
      <div class="element">
        <img src="./assets/bolso.jpeg" alt="Creation 1" />
        <div id="productName">Nombre del producto</div>
        <div id="productPrice">Precio X€</div>
      </div>
      <div class="element">
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
  gap: 10px;
  width: calc(100vw - 160px);
}
.element {
  display: flex;
  flex-direction: column;
  align-items: center;
  flex: 1;
  margin: 10px;
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