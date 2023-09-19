<template>
    <div class="container">
        <div class="info">
            <div class="bar left">
                <button>Términos generales y condiciones</button>
                <button>Politica de confidencialidad</button>
                <button>Entregas y devoluciones</button>
                <button>La marca</button>
                <button>Contactar</button>
            </div>
            <img src="../assets/FooterLogo.svg" alt="Monique Couture logo" />
            <div class="bar right">
                <button>Biblioteca de telas</button>
                <button>Encargos</button>
                <button>Tarjeta de regalo</button>
                <button>Mi cuenta</button>
            </div>
        </div>
        <div class="end">
            <div>2023, Nuria Arroyo Porras</div>
            <div class="rrss">
                <img src="./assets/ig.png" alt="Instagram logo" />
                <img src="./assets/fb.png" alt="Facebook logo" />
                <img src="./assets/pinterest.png" alt="Pinterest logo" />
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    background-color: var(--accent);
    color: var(--accent-typo);
    width: 100vw;
    height: fit-content;
    padding: 10px;
    text-align: center;
    margin: 0 auto;
    gap: 20px;
}

.info {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin: 40px 120px;
}

.info img {
    width: 20%;
}

.bar {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.bar button {
    border: none;
    background-color: transparent;
    color: var(--accent-typo);
    font-size: 1em;
}

.bar.left button{
    text-align: left;
}

.bar.right button{
    text-align: right;
}
.end {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin: 20px;
    font-size: 0.8em;
    font-weight: 100;
}

.rrss {
    display: flex;
    flex-direction: row;
    gap: 10px;
}
.rrss img {
    width: 20px;
}
</style>