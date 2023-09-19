<template>
    <div class="background">
        <div class="left">
            <div><img src="./assets/bolso.jpeg" alt="placeholder" /></div>
            <div><img src="./assets/bolso.jpeg" alt="placeholder" /></div>
        </div>
        <div class="right">
            <div><img src="./assets/bolso.jpeg" alt="placeholder" /></div>
        </div>
    </div>
</template>

<style scoped>
.background {
    display: flex;
    width: calc(100vw - 160px);
    height: 100vh;
    gap: 15px;
}

.left {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 15px;
    width: 20%;
    height: 100%;
    overflow: hidden;
    border: 1px solid black;
}

.right {
    flex: 2;
    display: flex;
    border: 1px solid black;
    width: 80%;
    height: 100%;
    overflow: hidden;
}

.left img, .right img {
    height: auto;
}
</style>