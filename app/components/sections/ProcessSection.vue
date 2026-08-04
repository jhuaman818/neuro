<template>
    <section class="process-section">
        <div class="process-content">
            <div>
                <span class="eyebrow">Metodo</span>
                <h2 class="process-title">Un proceso simple para avanzar con precision</h2>
                <p class="process-description">
                    Aterrizamos la idea, priorizamos lo importante y construimos por etapas para que cada decision tenga
                    impacto real.
                </p>
            </div>

            <div class="process-steps">
                <div class="process-step">
                    <span>01</span>
                    <h3>Diagnostico</h3>
                    <p>Entendemos objetivos, usuarios, procesos actuales y oportunidades de mejora.</p>
                </div>
                <div class="process-step">
                    <span>02</span>
                    <h3>Diseno funcional</h3>
                    <p>Definimos estructura, pantallas, integraciones y alcance con entregables claros.</p>
                </div>
                <div class="process-step">
                    <span>03</span>
                    <h3>Construccion</h3>
                    <p>Desarrollamos, probamos y ajustamos con avances visibles durante todo el proyecto.</p>
                </div>
                <div class="process-step">
                    <span>04</span>
                    <h3>Lanzamiento</h3>
                    <p>Publicamos, medimos y dejamos una base lista para iterar sin depender del azar.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.process-section {
    padding: 82px 24px;
    background: linear-gradient(135deg, #0b1720, #12202b);
    color: #ffffff;
}

.process-content {
    display: grid;
    grid-template-columns: minmax(0, 0.82fr) minmax(0, 1.18fr);
    gap: 44px;
    align-items: start;
    max-width: 1180px;
    margin: 0 auto;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 14px;
    padding: 7px 12px;
    border-radius: 999px;
    background: rgba(120, 242, 255, 0.12);
    color: #78f2ff;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.1em;
    text-transform: uppercase;
}

.process-title {
    margin: 0;
    font-size: clamp(2rem, 4vw, 3.1rem);
    line-height: 1.07;
}

.process-description {
    margin: 18px 0 0;
    color: rgba(255, 255, 255, 0.68);
    line-height: 1.75;
}

.process-steps {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 16px;
}

.process-step {
    min-height: 190px;
    padding: 24px;
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.06);
}

.process-step span {
    color: #78f2ff;
    font-weight: 900;
}

.process-step h3 {
    margin: 18px 0 10px;
    font-size: 1.25rem;
}

.process-step p {
    margin: 0;
    color: rgba(255, 255, 255, 0.66);
    line-height: 1.6;
}

@media (max-width: 900px) {
    .process-content {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 640px) {
    .process-section {
        padding: 56px 16px;
    }

    .process-steps {
        grid-template-columns: 1fr;
    }
}
</style>
