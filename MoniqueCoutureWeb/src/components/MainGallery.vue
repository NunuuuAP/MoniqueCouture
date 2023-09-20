<template>
    <div class="gallery">
        <div class="left">
            <div>Aquí van imágenes</div>
            <div>Aquí van imágenes</div>
        </div>
        <div class="right">
            Aquí van imágenes
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
    background-color:aqua;
}

.right {
    flex: 2;
    height: auto;
    background-color:aquamarine;

}

</style>