<template>
    <div class="background">
        <div class="left">
            <img src="./assets/bolso.jpeg" alt="Descripción del bolso" />
            <img src="./assets/bolso.jpeg" alt="Descripción del bolso" />
        </div>
        <div class="right">
            <img src="./assets/bolso.jpeg" alt="Descripción del bolso" />
        </div>
    </div>
</template>

<style scoped>
.background {
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
    justify-content: space-between;
    gap: 15px;
    width: 20%;
}

.right {
    flex: 2;
    height: auto;
    overflow: hidden;
}

.left img, .right img {
    object-fit: cover;
}

</style>