<template>
    <section>
        <h1>Formulario de contacto</h1>
        <div class="info">
            <div class="element">
                <p>Nombre*</p>
                <input type="text" placeholder="Nombre">
            </div>
            <div class="element">
                <p>Email*</p>
                <input type="email" placeholder="Email">
            </div>
            <div class="element">
                <p>Teléfono:</p>
                <input type="number" placeholder="Teléfono">
            </div>
        </div>
        <div id="message">
            <div class="element">
                <p>Asunto:</p>
                <input type="text" placeholder="Asunto del mensaje">
            </div>
            <div class="element">
                <p>Cuéntanos aquí tus dudas o comentarios*</p>
                <textarea rows="6" placeholder="Escribe aquí tu mensaje"></textarea>
            </div>
        </div>

        <p>*Estos apartados son obligatorios para poder enviar tu mensaje.</p>

    </section>
</template>

<style scoped>
section {
    display: flex;
    flex-direction: column;
    min-height: 40vh;
    padding: 50px 50px;
    gap: 20px;
}

section p {
    font-size: 0.8em;
}

.info {
    display: flex;
    flex-direction: row;
    width: 100%;
    gap: 20px;
}

.element {
    flex: 1;
}

section input {
    width: 100%;
    padding: 10px;
}

#message {
    display: flex;
    flex-direction: column;
    width: 100%;
    gap: 20px;
}

#message textarea {
    width: 100%;
    min-height: 3em;
    padding: 10px;
    resize: vertical;
    overflow: auto;
    font-family: inherit;
}
</style>