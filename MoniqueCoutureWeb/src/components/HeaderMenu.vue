<template>
    <div class="background">
        <menu>
            <img src="../assets/LogoPruebas.png" alt="Monique Couture logo" />
            <RouterLink to="/">Inicio</RouterLink>
            <RouterLink to="/orders">Encargos</RouterLink>
            <RouterLink to="/fabrics">Tejidos</RouterLink>
            <RouterLink to="/about">Sobre nosotros</RouterLink>
            <RouterLink to="/account">Mi cuenta</RouterLink>
        </menu>
    </div>
</template>

<style scoped>
.background {
    position: sticky;
    top: 0;
    display: flex;
    flex-direction: row;
    gap: 50px;
    justify-content: space-around;
    background-color: var(--background);
    color: var(--typo);
    width: 100vw;
    height: fit-content;
    padding: 50px 0 30px 0;
    text-align: center;
}

button {
    border: none;
    background-color: transparent;
    color: var(--typo);
    font-size: 1.1em;
    font-weight: bold;
}
</style>