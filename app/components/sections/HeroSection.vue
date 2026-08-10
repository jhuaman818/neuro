<template>
    <section class="hero-section">
        <div class="hero-shell">
            <div class="hero-content">
                <span class="eyebrow">Transformación Digital Inteligente</span>
                <h3 class="hero-title">Soluciones Digitales Completas para tu Negocio</h3>
                <p class="hero-description">
                    En Neurolink desarrollamos sistemas inteligentes, páginas web de alto rendimiento, CRM avanzados, bots de WhatsApp, automatizaciones empresariales y aplicaciones móviles que potencian tu negocio en la era digital.
                </p>

                <div class="hero-actions">
                    <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="hero-button primary">
                        Cotizar proyecto
                    </a>
                    <NuxtLink to="/portafolio" class="hero-button secondary">Ver trabajos</NuxtLink>
                </div>

                <div class="hero-metrics" aria-label="Indicadores de servicio">
                    <div>
                        <div class="metric-icon">✓</div>
                        <strong>+20</strong>
                        <span>soluciones implementadas</span>
                    </div>
                    <div>
                        <div class="metric-icon">⚡</div>
                        <strong>100%</strong>
                        <span>disponibilidad 24/7</span>
                    </div>
                    <div>
                        <div class="metric-icon">🚀</div>
                        <strong>3x</strong>
                        <span>canales integrados</span>
                    </div>
                </div>

                <div class="hero-benefits">
                    <div class="benefit-item">
                        <span class="benefit-icon">📊</span>
                        <p>Análisis de datos en tiempo real</p>
                    </div>
                    <div class="benefit-item">
                        <span class="benefit-icon">🔒</span>
                        <p>Seguridad empresarial</p>
                    </div>
                    <div class="benefit-item">
                        <span class="benefit-icon">⚙️</span>
                        <p>Escalabilidad garantizada</p>
                    </div>
                </div>
            </div>

            <div class="hero-visual" aria-label="Panel digital Neurolink">
                <div class="dashboard-panel">
                    <div class="panel-top">
                        <span class="dot red"></span>
                        <span class="dot yellow"></span>
                        <span class="dot green"></span>
                        <span class="panel-title">main.ts</span>
                    </div>
                    <div class="code-block">
                        <div class="code-line">
                            <span class="line-num">1</span>
                            <span class="keyword">import</span> { <span class="class">Innovation</span> } <span class="keyword">from</span> <span class="string">'@neurolink/core'</span>
                        </div>
                        <div class="code-line">
                            <span class="line-num">2</span>
                        </div>
                        <div class="code-line">
                            <span class="line-num">3</span>
                            <span class="keyword">const</span> <span class="variable">Future</span> = () =&gt; {
                        </div>
                        <div class="code-line">
                            <span class="line-num">4</span>
                            &nbsp;&nbsp;<span class="keyword">return</span> (&lt;<span class="class">DigitalTransformation</span> /&gt;);
                        </div>
                        <div class="code-line">
                            <span class="line-num">5</span>
                            }
                        </div>
                    </div>
                    <div class="compile-progress">
                        <div class="progress-bar">
                            <div class="progress-fill"></div>
                        </div>
                        <span class="progress-text">Compiling...</span>
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
    padding: 80px 24px 60px;
    background:
        radial-gradient(circle at 20% 30%, rgba(0, 200, 200, 0.3), transparent 35%),
        radial-gradient(circle at 85% 15%, rgba(0, 123, 255, 0.25), transparent 35%),
        radial-gradient(circle at 50% 100%, rgba(0, 166, 166, 0.15), transparent 40%),
        linear-gradient(135deg, #f0fafb 0%, #ffffff 50%, #e8f3f7 100%);
    border-top: 1px solid rgba(0, 123, 255, 0.1);
}

.hero-section::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        radial-gradient(circle at 30% 40%, rgba(0, 200, 200, 0.08) 0%, transparent 50%),
        linear-gradient(90deg, rgba(0, 123, 255, 0.03) 1px, transparent 1px),
        linear-gradient(0deg, rgba(0, 123, 255, 0.03) 1px, transparent 1px);
    background-size: auto, 60px 60px, 60px 60px;
    mask-image: linear-gradient(180deg, #000 0%, transparent 85%);
    opacity: 0.7;
}

.hero-shell {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 1.1fr) minmax(380px, 1fr);
    align-items: flex-start;
    gap: 48px;
    max-width: 1280px;
    margin: 0 auto;
}

.hero-content {
    max-width: 660px;
    padding-top: 20px;
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
    color: #08172b;
    font-size: clamp(1.8rem, 5.5vw, 4.5rem);
    line-height: 1;
    letter-spacing: -0.02em;
    font-weight: 900;
    background: linear-gradient(135deg, #08172b 0%, #0068d9 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.hero-description {
    max-width: 600px;
    margin: 22px 0 0;
    color: #3d4f5c;
    font-size: 1.05rem;
    line-height: 1.8;
    font-weight: 500;
}

.hero-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    margin-top: 32px;
    align-items: center;
}

.hero-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 56px;
    padding: 0 28px;
    border-radius: 10px;
    font-weight: 800;
    font-size: 1.02rem;
    text-decoration: none;
    transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease;
    cursor: pointer;
}

.hero-button:hover {
    transform: translateY(-4px);
}

.hero-button.primary {
    background: linear-gradient(135deg, #007bff 0%, #0a5fc4 100%);
    color: #ffffff;
    box-shadow: 0 24px 48px rgba(0, 123, 255, 0.32);
    font-weight: 900;
}

.hero-button.primary:hover {
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.42);
}

.hero-button.secondary {
    border: 2px solid #0068d9;
    background: transparent;
    color: #0068d9;
    font-weight: 800;
}

.hero-button.secondary:hover {
    background: rgba(0, 123, 255, 0.08);
}

.hero-metrics {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 8px;
    margin-top: 18px;
}

.hero-metrics div {
    padding: 14px 12px;
    border: 1px solid rgba(0, 123, 255, 0.15);
    border-radius: 10px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9), rgba(240, 250, 251, 0.8));
    backdrop-filter: blur(10px);
    box-shadow: 0 4px 12px rgba(0, 123, 255, 0.08);
    transition: all 0.3s ease;
    text-align: center;
    animation: slideUp 0.6s ease-out backwards;
}

.hero-metrics div:nth-child(1) {
    animation-delay: 0.1s;
}

.hero-metrics div:nth-child(2) {
    animation-delay: 0.2s;
}

.hero-metrics div:nth-child(3) {
    animation-delay: 0.3s;
}

.hero-metrics div:hover {
    transform: translateY(-6px);
    box-shadow: 0 12px 32px rgba(0, 123, 255, 0.15);
    border-color: rgba(0, 123, 255, 0.25);
}

@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.hero-metrics strong,
.hero-metrics span {
    display: block;
}

.hero-metrics strong {
    color: #12202b;
    font-size: 1.4rem;
    line-height: 1;
}

.metric-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 36px;
    height: 36px;
    border-radius: 8px;
    background: linear-gradient(135deg, rgba(0, 123, 255, 0.15), rgba(0, 200, 200, 0.15));
    font-size: 1.3rem;
    margin-bottom: 6px;
    animation: pulse 2s ease-in-out infinite;
}

@keyframes pulse {
    0%, 100% {
        transform: scale(1);
        opacity: 1;
    }
    50% {
        transform: scale(1.1);
        opacity: 0.8;
    }
}

.hero-benefits {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 8px;
    margin-top: 14px;
}

.benefit-item {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 10px 12px;
    border-radius: 10px;
    background: linear-gradient(135deg, rgba(0, 200, 200, 0.1), rgba(0, 123, 255, 0.1));
    border: 1px solid rgba(0, 200, 200, 0.2);
    transition: all 0.3s ease;
}

.benefit-item:hover {
    transform: translateX(6px);
    background: linear-gradient(135deg, rgba(0, 200, 200, 0.15), rgba(0, 123, 255, 0.15));
    border-color: rgba(0, 123, 255, 0.3);
}

.benefit-icon {
    font-size: 1.6rem;
    min-width: 28px;
}

.benefit-item p {
    margin: 0;
    color: #3d4f5c;
    font-size: 0.88rem;
    font-weight: 600;
    line-height: 1.3;
}

.hero-metrics span {
    margin-top: 4px;
    color: #3d4f5c;
    font-size: 0.82rem;
    line-height: 1.3;
    font-weight: 500;
}

.hero-visual {
    position: relative;
    min-height: 500px;
}

.dashboard-panel {
    position: absolute;
    inset: 20px 0 30px 0;
    margin: 0 auto;
    width: 95%;
    max-width: 520px;
    padding: 28px;
    border: 1.5px solid rgba(0, 200, 200, 0.3);
    border-radius: 12px;
    background:
        linear-gradient(145deg, rgba(5, 18, 28, 0.96), rgba(8, 40, 60, 0.92)),
        #091a28;
    box-shadow: 0 40px 100px rgba(0, 123, 255, 0.25), inset 0 1px 0 rgba(120, 242, 255, 0.1);
    overflow: hidden;
    left: 0;
    right: 0;
}

.dashboard-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(0, 200, 200, 0.06) 1px, transparent 1px),
        linear-gradient(0deg, rgba(0, 200, 200, 0.06) 1px, transparent 1px);
    background-size: 42px 42px;
    pointer-events: none;
}

.panel-top,
.chart-block,
.status-grid {
    position: relative;
    z-index: 1;
}

.panel-top {
    display: flex;
    align-items: center;
    gap: 12px;
    padding-bottom: 16px;
    border-bottom: 1px solid rgba(0, 200, 200, 0.1);
}

.dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    flex-shrink: 0;
}

.dot.red {
    background: #ff5f57;
}

.dot.yellow {
    background: #ffbd2e;
}

.dot.green {
    background: #28c940;
}

.panel-title {
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.6);
    font-weight: 600;
    margin-left: 8px;
}

.code-block {
    margin: 20px 0;
    font-family: 'Monaco', 'Menlo', 'Ubuntu Mono', monospace;
    font-size: 0.92rem;
    line-height: 1.6;
    color: rgba(255, 255, 255, 0.8);
}

.code-line {
    display: flex;
    align-items: center;
    gap: 16px;
    padding: 2px 0;
    color: rgba(255, 255, 255, 0.7);
}

.line-num {
    color: rgba(255, 255, 255, 0.35);
    font-weight: 500;
    min-width: 32px;
    text-align: right;
}

.keyword {
    color: #ff79c6;
    font-weight: 600;
}

.class {
    color: #50fa7b;
    font-weight: 600;
}

.variable {
    color: #8be9fd;
    font-weight: 600;
}

.string {
    color: #f1fa8c;
}

.compile-progress {
    margin: 20px 0;
    padding: 12px 0;
    border-top: 1px solid rgba(0, 200, 200, 0.1);
    border-bottom: 1px solid rgba(0, 200, 200, 0.1);
}

.progress-bar {
    width: 100%;
    height: 6px;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 3px;
    overflow: hidden;
    margin-bottom: 8px;
}

.progress-fill {
    height: 100%;
    width: 65%;
    background: linear-gradient(90deg, #00d4ff, #00a6a6);
    border-radius: 3px;
    box-shadow: 0 0 12px rgba(0, 212, 255, 0.5);
    animation: progress-pulse 2s ease-in-out infinite;
}

@keyframes progress-pulse {
    0%, 100% {
        width: 65%;
    }
    50% {
        width: 75%;
    }
}

.progress-text {
    font-size: 0.78rem;
    color: #00d4ff;
    font-weight: 700;
    letter-spacing: 0.05em;
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
    width: 220px;
    padding: 20px;
    border: 1.5px solid rgba(0, 123, 255, 0.25);
    border-radius: 10px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.96), rgba(240, 250, 251, 0.92));
    box-shadow: 0 28px 64px rgba(0, 123, 255, 0.22), inset 0 1px 0 rgba(255, 255, 255, 0.8);
    backdrop-filter: blur(20px);
    transition: all 0.3s ease;
}

.floating-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 40px 80px rgba(0, 123, 255, 0.32), inset 0 1px 0 rgba(255, 255, 255, 0.8);
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
    top: -30px;
    left: -40px;
}

.card-two {
    right: -40px;
    bottom: -20px;
}

@media (max-width: 960px) {
    .hero-section {
        padding-top: 48px;
    }

    .hero-shell {
        grid-template-columns: 1fr;
        gap: 36px;
    }

    .hero-content {
        max-width: none;
    }

    .hero-visual {
        min-height: 400px;
    }

    .dashboard-panel {
        inset: 20px 0;
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

    .hero-benefits {
        grid-template-columns: 1fr;
    }

    .hero-visual {
        min-height: 360px;
    }

    .dashboard-panel {
        inset: 32px 0 20px;
        padding: 16px;
    }

    .code-block {
        font-size: 0.8rem;
        margin: 12px 0;
    }

    .code-line {
        gap: 8px;
    }

    .line-num {
        min-width: 24px;
    }

    .compile-progress {
        margin: 12px 0;
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
