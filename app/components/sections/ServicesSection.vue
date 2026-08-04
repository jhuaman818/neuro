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
    padding: 82px 24px;
    background: #ffffff;
}

.services-content {
    max-width: 1180px;
    margin: 0 auto;
}

.section-heading {
    max-width: 780px;
    margin: 0 auto 42px;
    text-align: center;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 14px;
    padding: 7px 12px;
    border-radius: 999px;
    background: rgba(0, 166, 166, 0.1);
    color: #008484;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.1em;
    text-transform: uppercase;
}

.services-title {
    margin: 0;
    color: #12202b;
    font-size: clamp(2rem, 4vw, 3.35rem);
    line-height: 1.06;
}

.services-description {
    margin: 18px auto 0;
    color: #5f6f7b;
    font-size: 1.05rem;
    line-height: 1.7;
}

.services-list {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}

.service-item {
    position: relative;
    min-height: 320px;
    padding: 28px;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background:
        linear-gradient(180deg, rgba(245, 251, 252, 0.92), rgba(255, 255, 255, 1)),
        #ffffff;
    box-shadow: 0 18px 44px rgba(18, 32, 43, 0.07);
    overflow: hidden;
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
    width: 50px;
    height: 50px;
    border-radius: 8px;
    background: #12202b;
    color: #78f2ff;
    font-weight: 900;
}

.service-title {
    margin: 24px 0 12px;
    color: #12202b;
    font-size: 1.45rem;
}

.service-description {
    margin: 0;
    color: #5f6f7b;
    line-height: 1.68;
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
