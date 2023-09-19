<template>
    <div class="gallery">
        <div class="left">
            <div>hola</div>
            <div>adios</div>
        </div>
        <div class="right">
        </div>
    </div>
</template>

<style scoped>
.gallery {
    display: flex;
    width: calc(100vw - 160px);
    height: 80vh;
    gap: 15px;
    object-fit: cover;
}
.left {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 15px;
    width: 100%;
    height: 100%;
}

.left div {
    flex: 1;
    background-color: blue;
}

.right {
    flex: 2;
    height: auto;
    background-color: red;

}

</style>