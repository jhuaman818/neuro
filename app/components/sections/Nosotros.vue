<template>
    <main class="about-page">
        <section class="about-hero">
            <span class="eyebrow">Nosotros</span>
            <h1>Neurolink es mi proyecto como desarrollador independiente</h1>
            <p>
                Estoy iniciando este camino solo, construyendo soluciones web prácticas y modernas para pequeñas empresas,
                emprendedores y marcas que necesitan presencia digital real.
            </p>
        </section>

        <section class="about-grid">
            <article class="about-card">
                <h2>Trabajo directo contigo</h2>
                <p>
                    Cada proyecto lo atiendo personalmente. Esto significa comunicación rápida, entregas claras y una
                    solución hecha a tu medida.
                </p>
            </article>

            <article class="about-card">
                <h2>Herramientas reales</h2>
                <p>
                    Desarrollo con Vue.js, Laravel, PHP, Node.js, bases de datos y despliegue en servidores para que tu
                    sitio funcione bien desde el primer día.
                </p>
            </article>

            <article class="about-card">
                <h2>Proyectos simples, resultados profesionales</h2>
                <p>
                    Me enfoco en lo que realmente importa: diseño limpio, experiencia de usuario y una solución que sea fácil
                    de mantener y escalar.
                </p>
            </article>
        </section>

        <section class="about-extra">
            <div class="about-extra-card">
                <h3>¿Por qué elegir Neurolink?</h3>
                <p>
                    Porque recibes atención personalizada de un desarrollador que entiende tu negocio y está dispuesto a
                    crecer contigo, proyecto por proyecto.
                </p>
            </div>

            <div class="about-extra-card">
                <h3>¿Qué puedo hacer por ti?</h3>
                <ul>
                    <li>Páginas web corporativas y landing pages</li>
                    <li>Integraciones con APIs y WhatsApp</li>
                    <li>Servicios backend con Laravel y PHP</li>
                    <li>Despliegue y mantenimiento en VPS</li>
                </ul>
            </div>
        </section>

        <section class="about-cta">
            <p>
                Si estás empezando un proyecto o necesitas mejorar tu presencia digital, hablemos. Estoy listo para
                ayudarte a transformar tu idea en una web profesional.
            </p>
            <NuxtLink to="/contacto" class="button">Contactar ahora</NuxtLink>
        </section>
    </main>
</template>

<style scoped>
.about-page {
    position: relative;
    overflow: hidden;
    max-width: 1280px;
    margin: 0 auto;
    padding: 100px 24px 60px;
    display: grid;
    gap: 48px;
    background:
        radial-gradient(circle at 20% 30%, rgba(0, 200, 200, 0.25), transparent 35%),
        radial-gradient(circle at 80% 70%, rgba(0, 123, 255, 0.2), transparent 40%),
        linear-gradient(135deg, #f0fafb 0%, #ffffff 50%, #e8f3f7 100%);
    border-radius: 0;
    border: none;
    box-shadow: none;
    color: #08172b;
}

.about-page::before {
    content: '';
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(0, 200, 200, 0.05) 1px, transparent 1px),
        linear-gradient(0deg, rgba(0, 200, 200, 0.05) 1px, transparent 1px),
        radial-gradient(circle at 15% 10%, rgba(0, 200, 200, 0.15), transparent 20%),
        radial-gradient(circle at 80% 25%, rgba(0, 123, 255, 0.12), transparent 25%);
    background-size: 50px 50px, 50px 50px, 100% 100%, 100% 100%;
    opacity: 1;
    pointer-events: none;
    mask-image: linear-gradient(180deg, #000 0%, transparent 90%);
}

.about-page::after {
    content: '';
    position: absolute;
    inset: 0;
    background:
        radial-gradient(circle at 24% 82%, rgba(0, 123, 255, 0.08), transparent 15%),
        radial-gradient(circle at 75% 24%, rgba(0, 200, 200, 0.08), transparent 15%);
    opacity: 1;
    pointer-events: none;
}

.about-hero {
    position: relative;
    z-index: 1;
    max-width: 730px;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 18px;
    padding: 8px 16px;
    border-radius: 999px;
    background: linear-gradient(135deg, rgba(0, 200, 200, 0.15), rgba(0, 123, 255, 0.15));
    color: #00a6a6;
    font-size: 0.78rem;
    font-weight: 900;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    border: 1px solid rgba(0, 200, 200, 0.2);
}

.about-hero h1 {
    margin: 0;
    color: #08172b;
    font-size: clamp(2.4rem, 5vw, 3.8rem);
    line-height: 1.1;
    font-weight: 900;
    background: linear-gradient(135deg, #08172b 0%, #0068d9 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.about-hero p {
    max-width: 620px;
    margin: 22px 0 0;
    color: #3d4f5c;
    font-size: 1.05rem;
    line-height: 1.8;
    font-weight: 500;
}

.about-grid {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
}

.about-card {
    padding: 32px;
    border-radius: 12px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95), rgba(240, 250, 251, 0.9));
    border: 1.5px solid rgba(0, 200, 200, 0.2);
    box-shadow: 0 20px 48px rgba(0, 123, 255, 0.12), inset 0 1px 0 rgba(255, 255, 255, 0.8);
    transition: all 0.3s ease;
}

.about-card:hover {
    transform: translateY(-8px);
    border-color: rgba(0, 123, 255, 0.3);
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.18), inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

.about-card h2 {
    margin: 0 0 16px;
    font-size: 1.3rem;
    color: #08172b;
    font-weight: 800;
}

.about-card p {
    margin: 0;
    color: #3d4f5c;
    line-height: 1.78;
    font-weight: 500;
}

.about-extra {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    gap: 24px;
}

.about-extra-card {
    padding: 32px;
    border-radius: 12px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95), rgba(240, 250, 251, 0.9));
    border: 1.5px solid rgba(0, 200, 200, 0.2);
    box-shadow: 0 20px 48px rgba(0, 123, 255, 0.12), inset 0 1px 0 rgba(255, 255, 255, 0.8);
    transition: all 0.3s ease;
}

.about-extra-card:hover {
    transform: translateY(-8px);
    border-color: rgba(0, 123, 255, 0.3);
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.18), inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

.about-extra-card h3 {
    margin: 0 0 16px;
    color: #08172b;
    font-size: 1.25rem;
    font-weight: 800;
}

.about-extra-card p,
.about-extra-card ul {
    margin: 0;
    color: #3d4f5c;
    line-height: 1.78;
    font-weight: 500;
}

.about-extra-card ul {
    padding-left: 18px;
}

.about-extra-card li {
    margin-bottom: 10px;
}

.about-cta {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 1fr) auto;
    align-items: center;
    gap: 28px;
    padding: 36px;
    border-radius: 12px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.96), rgba(240, 250, 251, 0.92));
    border: 1.5px solid rgba(0, 123, 255, 0.25);
    box-shadow: 0 24px 56px rgba(0, 123, 255, 0.15), inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

.about-cta p {
    margin: 0;
    color: #3d4f5c;
    font-size: 1.05rem;
    line-height: 1.8;
    font-weight: 500;
}

.button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 56px;
    padding: 0 28px;
    border-radius: 10px;
    background: linear-gradient(135deg, #007bff 0%, #0a5fc4 100%);
    color: #ffffff;
    font-weight: 900;
    font-size: 1.02rem;
    text-decoration: none;
    box-shadow: 0 24px 48px rgba(0, 123, 255, 0.32);
    transition: all 0.3s ease;
    white-space: nowrap;
}

.button:hover {
    transform: translateY(-4px);
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.42);
}

@media (max-width: 980px) {
    .about-grid,
    .about-extra,
    .about-cta {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 640px) {
    .about-page {
        padding: 56px 18px 36px;
    }

    .about-card,
    .about-extra-card,
    .about-cta {
        padding: 22px;
    }
}
</style>