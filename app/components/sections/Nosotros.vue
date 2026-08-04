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
    max-width: 1180px;
    margin: 0 auto;
    padding: 80px 24px 48px;
    display: grid;
    gap: 36px;
    background: linear-gradient(180deg, #f8fafc 0%, #e8f1fb 100%);
    border-radius: 32px;
    border: 1px solid rgba(148, 163, 184, 0.18);
    box-shadow: 0 36px 80px rgba(15, 23, 42, 0.08);
    color: #0f172a;
}

.about-page::before {
    content: '';
    position: absolute;
    inset: 0;
    background-image:
        linear-gradient(90deg, rgba(15, 23, 42, 0.04) 1px, transparent 1px),
        linear-gradient(180deg, rgba(15, 23, 42, 0.04) 1px, transparent 1px),
        radial-gradient(circle at 15% 10%, rgba(14, 165, 233, 0.18), transparent 12%),
        radial-gradient(circle at 80% 25%, rgba(96, 165, 250, 0.14), transparent 14%);
    background-size: 100% 100%, 100% 100%, 320px 320px, 320px 320px;
    opacity: 0.55;
    pointer-events: none;
}

.about-page::after {
    content: '';
    position: absolute;
    inset: 0;
    background-image:
        radial-gradient(circle at 24% 82%, rgba(59, 130, 246, 0.06), transparent 10%),
        radial-gradient(circle at 75% 24%, rgba(14, 165, 233, 0.07), transparent 9%);
    opacity: 0.35;
    pointer-events: none;
}

.about-hero {
    max-width: 730px;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 16px;
    padding: 8px 16px;
    border-radius: 999px;
    background: rgba(59, 130, 246, 0.12);
    color: #1d4ed8;
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 0.12em;
    text-transform: uppercase;
}

.about-hero h1 {
    margin: 0;
    color: #0f172a;
    font-size: clamp(2.4rem, 4vw, 3.6rem);
    line-height: 1.02;
}

.about-hero p {
    max-width: 620px;
    margin: 18px 0 0;
    color: rgba(15, 23, 42, 0.72);
    font-size: 1rem;
    line-height: 1.8;
}

.about-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}

.about-card {
    padding: 28px 26px;
    border-radius: 24px;
    background: #ffffff;
    border: 1px solid rgba(148, 163, 184, 0.18);
    box-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
}

.about-card h2 {
    margin: 0 0 14px;
    font-size: 1.2rem;
    color: #0f172a;
}

.about-card p {
    margin: 0;
    color: rgba(15, 23, 42, 0.72);
    line-height: 1.75;
}

.about-extra {
    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    gap: 20px;
}

.about-extra-card {
    padding: 28px 30px;
    border-radius: 24px;
    background: #ffffff;
    border: 1px solid rgba(148, 163, 184, 0.16);
    box-shadow: 0 18px 40px rgba(15, 23, 42, 0.06);
}

.about-extra-card h3 {
    margin: 0 0 14px;
    color: #0f172a;
    font-size: 1.15rem;
}

.about-extra-card p,
.about-extra-card ul {
    margin: 0;
    color: rgba(15, 23, 42, 0.72);
    line-height: 1.75;
}

.about-extra-card ul {
    padding-left: 18px;
}

.about-extra-card li {
    margin-bottom: 10px;
}

.about-cta {
    display: grid;
    grid-template-columns: minmax(0, 1fr) auto;
    align-items: center;
    gap: 24px;
    padding: 28px 30px;
    border-radius: 24px;
    background: #ffffff;
    border: 1px solid rgba(148, 163, 184, 0.16);
    box-shadow: 0 20px 48px rgba(15, 23, 42, 0.08);
}

.about-cta p {
    margin: 0;
    color: rgba(15, 23, 42, 0.82);
    font-size: 1rem;
    line-height: 1.8;
}

.button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 48px;
    padding: 0 22px;
    border-radius: 12px;
    background: linear-gradient(135deg, #0ea5e9, #3b82f6);
    color: #ffffff;
    font-weight: 800;
    text-decoration: none;
    box-shadow: 0 18px 36px rgba(14, 165, 233, 0.28);
    transition: transform 0.2s ease, background-color 0.2s ease;
}

.button:hover {
    transform: translateY(-2px);
    background: linear-gradient(135deg, #38bdf8, #60a5fa);
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