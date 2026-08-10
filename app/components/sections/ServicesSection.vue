<template>
    <section class="services-section">
        <div class="services-content">
            <div class="section-heading">
                <span class="eyebrow">Servicios</span>
                <h2 class="services-title">Servicios que ofrecemos</h2>
                <p class="services-description">
                    Atendemos necesidades reales de negocios: corregimos sistemas existentes, creamos presencia digital
                    y conectamos ventas, atencion y operaciones con tecnologia.
                </p>
            </div>

            <div class="services-list">
                <div class="service-item">
                    <span class="service-icon">01</span>
                    <h3 class="service-title">Correccion de bugs</h3>
                    <p class="service-description">
                        Revisamos y solucionamos errores en sistemas de facturacion electronica, integraciones,
                        reportes, flujos y procesos criticos.
                    </p>
                    <ul>
                        <li>Facturacion electronica</li>
                        <li>Soporte y mantenimiento</li>
                    </ul>
                </div>
                <div class="service-item">
                    <span class="service-icon">02</span>
                    <h3 class="service-title">Paginas web</h3>
                    <p class="service-description">
                        Disenamos paginas corporativas, sitios informativos y paginas comerciales listas para mostrar
                        servicios, captar clientes y posicionar marca.
                    </p>
                    <ul>
                        <li>Webs responsive</li>
                        <li>SEO tecnico basico</li>
                    </ul>
                </div>
                <div class="service-item">
                    <span class="service-icon">03</span>
                    <h3 class="service-title">Landing pages y fan pages</h3>
                    <p class="service-description">
                        Creamos paginas enfocadas en campanas, ventas, registros, promociones y presencia digital para
                        redes o negocios locales.
                    </p>
                    <ul>
                        <li>Campanas comerciales</li>
                        <li>Captacion de leads</li>
                    </ul>
                </div>
                <div class="service-item">
                    <span class="service-icon">04</span>
                    <h3 class="service-title">CRM para negocios</h3>
                    <p class="service-description">
                        Implementamos sistemas para ordenar clientes, ventas, seguimiento, tareas y oportunidades desde
                        un solo panel.
                    </p>
                    <ul>
                        <li>Gestion de clientes</li>
                        <li>Pipeline comercial</li>
                    </ul>
                </div>
                <div class="service-item">
                    <span class="service-icon">05</span>
                    <h3 class="service-title">Bots de WhatsApp</h3>
                    <p class="service-description">
                        Automatizamos respuestas, formularios, derivaciones y avisos para mejorar la atencion y no
                        perder consultas.
                    </p>
                    <ul>
                        <li>WhatsApp Business</li>
                        <li>Flujos automatizados</li>
                    </ul>
                </div>
                <div class="service-item">
                    <span class="service-icon">06</span>
                    <h3 class="service-title">Apps moviles y automatizacion</h3>
                    <p class="service-description">
                        Desarrollamos aplicaciones moviles y automatizaciones para reservas, pedidos, reportes,
                        notificaciones y operaciones internas.
                    </p>
                    <ul>
                        <li>Kotlin y soluciones moviles</li>
                        <li>Procesos conectados</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.services-section {
    position: relative;
    padding: 90px 24px;
    background:
        radial-gradient(circle at 10% 20%, rgba(0, 200, 200, 0.25), transparent 35%),
        radial-gradient(circle at 90% 80%, rgba(0, 123, 255, 0.2), transparent 40%),
        linear-gradient(135deg, #f0fafb 0%, #ffffff 50%, #e8f3f7 100%);
    border-top: 1px solid rgba(0, 123, 255, 0.08);
    border-bottom: 1px solid rgba(0, 200, 200, 0.08);
}

.services-section::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(0, 200, 200, 0.04) 1px, transparent 1px),
        linear-gradient(0deg, rgba(0, 200, 200, 0.04) 1px, transparent 1px);
    background-size: 50px 50px;
    pointer-events: none;
    mask-image: linear-gradient(180deg, #000 0%, transparent 90%);
}

.services-content {
    position: relative;
    z-index: 1;
    max-width: 1280px;
    margin: 0 auto;
}

.section-heading {
    max-width: 780px;
    margin: 0 auto 42px;
    text-align: center;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 16px;
    padding: 8px 14px;
    border-radius: 999px;
    background: linear-gradient(135deg, rgba(0, 200, 200, 0.15), rgba(0, 123, 255, 0.15));
    color: #00a6a6;
    font-size: 0.76rem;
    font-weight: 900;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    border: 1px solid rgba(0, 200, 200, 0.2);
}

.services-title {
    margin: 0;
    color: #08172b;
    font-size: clamp(2rem, 5vw, 3.5rem);
    line-height: 1.1;
    font-weight: 900;
    background: linear-gradient(135deg, #08172b 0%, #0068d9 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.services-description {
    margin: 18px auto 0;
    color: #3d4f5c;
    font-size: 1.05rem;
    line-height: 1.8;
    font-weight: 500;
}

.services-list {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
    margin-top: 8px;
}

.service-item {
    position: relative;
    min-height: 340px;
    padding: 32px;
    border: 1.5px solid rgba(0, 200, 200, 0.2);
    border-radius: 12px;
    background:
        linear-gradient(135deg, rgba(255, 255, 255, 0.95), rgba(240, 250, 251, 0.9)),
        #ffffff;
    box-shadow: 0 20px 48px rgba(0, 123, 255, 0.12), inset 0 1px 0 rgba(255, 255, 255, 0.8);
    overflow: hidden;
    transition: all 0.3s ease;
}

.service-item:hover {
    transform: translateY(-8px);
    border-color: rgba(0, 123, 255, 0.3);
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.18), inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

.service-item::after {
    content: "";
    position: absolute;
    right: -42px;
    top: -42px;
    width: 120px;
    height: 120px;
    border: 1px solid rgba(0, 123, 255, 0.18);
    border-radius: 50%;
}

.service-icon {
    display: grid;
    place-items: center;
    width: 56px;
    height: 56px;
    border-radius: 10px;
    background: linear-gradient(135deg, #007bff, #0068d9);
    color: #ffffff;
    font-weight: 900;
    font-size: 1.3rem;
    box-shadow: 0 8px 20px rgba(0, 123, 255, 0.25);
}

.service-title {
    margin: 26px 0 14px;
    color: #08172b;
    font-size: 1.48rem;
    font-weight: 800;
    line-height: 1.2;
}

.service-description {
    margin: 0;
    color: #3d4f5c;
    line-height: 1.72;
    font-weight: 500;
}

ul {
    display: grid;
    gap: 9px;
    margin: 22px 0 0;
    padding: 0;
    list-style: none;
}

li {
    display: flex;
    gap: 9px;
    color: #1d3442;
    font-size: 0.94rem;
    font-weight: 750;
}

li::before {
    content: "";
    width: 8px;
    height: 8px;
    margin-top: 7px;
    border-radius: 50%;
    background: #00a6a6;
    flex: 0 0 auto;
}

@media (max-width: 900px) {
    .services-list {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 640px) {
    .services-section {
        padding: 56px 16px;
    }
}
</style>
