<template>
    <section class="hero-section">
        <div class="hero-shell">
            <div class="hero-content">
                <span class="eyebrow">Soporte y desarrollo digital</span>
                <h1 class="hero-title">Soluciones web, facturacion, CRM, bots y apps para tu negocio</h1>
                <p class="hero-description">
                    En Neurolink corregimos bugs en sistemas de facturacion electronica y desarrollamos paginas web,
                    landing pages, fan pages, CRM, bots de WhatsApp, automatizaciones y aplicaciones moviles.
                </p>

                <div class="hero-actions">
                    <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="hero-button primary">
                        Cotizar proyecto
                    </a>
                    <NuxtLink to="/portafolio" class="hero-button secondary">Ver trabajos</NuxtLink>
                </div>

                <div class="hero-metrics" aria-label="Indicadores de servicio">
                    <div>
                        <strong>+20</strong>
                        <span>servicios digitales</span>
                    </div>
                    <div>
                        <strong>3x</strong>
                        <span>canales conectados</span>
                    </div>
                    <div>
                        <strong>24/7</strong>
                        <span>presencia digital</span>
                    </div>
                </div>
            </div>

            <div class="hero-visual" aria-label="Panel digital Neurolink">
                <div class="dashboard-panel">
                    <div class="panel-top">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <div class="chart-block">
                        <div class="chart-line line-one"></div>
                        <div class="chart-line line-two"></div>
                        <div class="chart-line line-three"></div>
                    </div>
                    <div class="status-grid">
                        <div class="status-card active">
                            <span>Web</span>
                            <strong>SEO</strong>
                        </div>
                        <div class="status-card">
                            <span>CRM</span>
                            <strong>Lead</strong>
                        </div>
                        <div class="status-card">
                            <span>Bot</span>
                            <strong>WA</strong>
                        </div>
                    </div>
                </div>
                <div class="floating-card card-one">
                    <span>Soporte</span>
                    <strong>Facturacion electronica</strong>
                </div>
                <div class="floating-card card-two">
                    <span>Desarrollo</span>
                    <strong>Web + App movil</strong>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.hero-section {
    position: relative;
    overflow: hidden;
    padding: 86px 24px 70px;
    background:
        radial-gradient(circle at 14% 18%, rgba(0, 166, 166, 0.2), transparent 28%),
        radial-gradient(circle at 86% 8%, rgba(0, 123, 255, 0.18), transparent 30%),
        linear-gradient(135deg, #f5fbfc 0%, #ffffff 46%, #eef5f8 100%);
}

.hero-section::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(18, 32, 43, 0.045) 1px, transparent 1px),
        linear-gradient(0deg, rgba(18, 32, 43, 0.045) 1px, transparent 1px);
    background-size: 54px 54px;
    mask-image: linear-gradient(180deg, #000 0%, transparent 82%);
}

.hero-shell {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 1fr) minmax(360px, 0.9fr);
    align-items: center;
    gap: 58px;
    max-width: 1180px;
    margin: 0 auto;
}

.hero-content {
    max-width: 660px;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 18px;
    padding: 8px 13px;
    border-radius: 999px;
    background: rgba(0, 123, 255, 0.1);
    color: #0068d9;
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 0.08em;
    text-transform: uppercase;
}

.hero-title {
    margin: 0;
    color: #12202b;
    font-size: clamp(2.65rem, 6vw, 5.15rem);
    line-height: 0.98;
    letter-spacing: 0;
}

.hero-description {
    max-width: 610px;
    margin: 24px 0 0;
    color: #5f6f7b;
    font-size: 1.12rem;
    line-height: 1.75;
}

.hero-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
    margin-top: 32px;
}

.hero-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 52px;
    padding: 0 22px;
    border-radius: 8px;
    font-weight: 850;
    text-decoration: none;
    transition: transform 0.2s ease, box-shadow 0.2s ease, background-color 0.2s ease;
}

.hero-button:hover {
    transform: translateY(-2px);
}

.hero-button.primary {
    background: linear-gradient(135deg, #007bff, #00a6a6);
    color: #ffffff;
    box-shadow: 0 18px 36px rgba(0, 123, 255, 0.24);
}

.hero-button.secondary {
    border: 1px solid rgba(18, 32, 43, 0.12);
    background: rgba(255, 255, 255, 0.82);
    color: #12202b;
}

.hero-metrics {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 14px;
    margin-top: 42px;
}

.hero-metrics div {
    padding: 16px;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.72);
}

.hero-metrics strong,
.hero-metrics span {
    display: block;
}

.hero-metrics strong {
    color: #12202b;
    font-size: 1.55rem;
    line-height: 1;
}

.hero-metrics span {
    margin-top: 8px;
    color: #657681;
    font-size: 0.88rem;
    line-height: 1.35;
}

.hero-visual {
    position: relative;
    min-height: 520px;
}

.dashboard-panel {
    position: absolute;
    inset: 30px 0 40px 18px;
    padding: 24px;
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 8px;
    background:
        linear-gradient(145deg, rgba(8, 22, 34, 0.94), rgba(13, 74, 94, 0.86)),
        #12202b;
    box-shadow: 0 34px 80px rgba(18, 32, 43, 0.28);
    overflow: hidden;
}

.dashboard-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(120, 242, 255, 0.08) 1px, transparent 1px),
        linear-gradient(0deg, rgba(120, 242, 255, 0.08) 1px, transparent 1px);
    background-size: 38px 38px;
}

.panel-top,
.chart-block,
.status-grid {
    position: relative;
    z-index: 1;
}

.panel-top {
    display: flex;
    gap: 8px;
}

.panel-top span {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.45);
}

.chart-block {
    height: 250px;
    margin-top: 34px;
    border: 1px solid rgba(120, 242, 255, 0.2);
    border-radius: 8px;
    background: rgba(7, 20, 32, 0.48);
}

.chart-line {
    position: absolute;
    left: 32px;
    right: 32px;
    height: 2px;
    background: linear-gradient(90deg, transparent, #78f2ff, transparent);
    transform-origin: left center;
}

.line-one {
    top: 34%;
    transform: rotate(-8deg);
}

.line-two {
    top: 52%;
    transform: rotate(12deg);
    opacity: 0.7;
}

.line-three {
    top: 70%;
    transform: rotate(-16deg);
    opacity: 0.55;
}

.status-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 12px;
    margin-top: 18px;
}

.status-card {
    padding: 16px;
    border: 1px solid rgba(255, 255, 255, 0.12);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.08);
    color: #ffffff;
}

.status-card.active {
    background: rgba(0, 166, 166, 0.22);
}

.status-card span,
.status-card strong {
    display: block;
}

.status-card span {
    color: rgba(255, 255, 255, 0.58);
    font-size: 0.76rem;
    font-weight: 800;
}

.status-card strong {
    margin-top: 8px;
    font-size: 1.35rem;
}

.floating-card {
    position: absolute;
    z-index: 2;
    width: 210px;
    padding: 18px;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.9);
    box-shadow: 0 24px 52px rgba(18, 32, 43, 0.16);
    backdrop-filter: blur(18px);
}

.floating-card span,
.floating-card strong {
    display: block;
}

.floating-card span {
    color: #0068d9;
    font-size: 0.75rem;
    font-weight: 850;
    letter-spacing: 0.08em;
    text-transform: uppercase;
}

.floating-card strong {
    margin-top: 8px;
    color: #12202b;
    font-size: 1.08rem;
}

.card-one {
    top: 0;
    left: 0;
}

.card-two {
    right: 0;
    bottom: 0;
}

@media (max-width: 960px) {
    .hero-section {
        padding-top: 58px;
    }

    .hero-shell {
        grid-template-columns: 1fr;
        gap: 34px;
    }

    .hero-content {
        max-width: none;
    }

    .hero-visual {
        min-height: 420px;
    }

    .dashboard-panel {
        inset: 26px 0;
    }
}

@media (max-width: 640px) {
    .hero-section {
        padding: 42px 16px 46px;
    }

    .hero-actions,
    .hero-button {
        width: 100%;
    }

    .hero-metrics {
        grid-template-columns: 1fr;
    }

    .hero-visual {
        min-height: 360px;
    }

    .dashboard-panel {
        inset: 32px 0 20px;
        padding: 18px;
    }

    .chart-block {
        height: 190px;
    }

    .floating-card {
        width: 170px;
        padding: 14px;
    }

    .card-two {
        right: 8px;
    }
}
</style>
