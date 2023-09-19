<template>
    <div class="background">
        <div class="left">
            <img src="./assets/bolso.jpeg" alt="placeholder" />
            <img src="./assets/bolso.jpeg" alt="placeholder" />
        </div>
        <div class="right">
            <img src="./assets/bolso.jpeg" alt="placeholder" />
        </div>
    </div>
</template>

<style scoped>
.background {
    display: flex;
    width: calc(100vw - 160px);
    height: 80vh;
    gap: 15px;
}

.left, .right {
    border-radius: 10px;
}

.left {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    gap: 15px;
    width: 20%;
    height: 100%;
}

.right {
    flex: 2;
    display: flex;
    width: 80%;
    height: 100%;
    overflow: hidden;
}

.left img {
    width: auto;
    height: fit-content;
    border-radius: 10px;
    object-fit: cover;
}

.right img {
    width: auto;
    height: fit-content;
    border-radius: 10px;
    object-fit: cover;
}

</style>