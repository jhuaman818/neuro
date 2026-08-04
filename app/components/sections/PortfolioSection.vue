<template>
    <section class="portfolio-section">
        <div class="portfolio-shell">
            <div class="portfolio-heading">
                <div>
                    <span class="eyebrow">Portafolio</span>
                    <h2 class="portfolio-title">Tipos de soluciones que podemos construir</h2>
                </div>
                <NuxtLink to="/portafolio" class="portfolio-link">Ver portafolio</NuxtLink>
            </div>

            <div class="portfolio-grid">
                <article class="portfolio-item" v-for="item in portfolioItems" :key="item.id">
                    <div class="portfolio-preview" :class="item.theme">
                        <span>{{ item.tag }}</span>
                    </div>
                    <div class="portfolio-body">
                        <h3 class="portfolio-item-title">{{ item.title }}</h3>
                        <p class="portfolio-item-description">{{ item.description }}</p>
                    </div>
                </article>
            </div>
        </div>
    </section>
</template>

<script setup>
const portfolioItems = [
    {
        id: 1,
        title: 'Correccion en facturacion electronica',
        description: 'Revision de errores, ajustes de flujos, reportes, integraciones y soporte para sistemas activos.',
        tag: 'Soporte',
        theme: 'theme-blue'
    },
    {
        id: 2,
        title: 'Pagina web o landing de ventas',
        description: 'Sitios modernos para presentar servicios, recibir consultas, lanzar campanas y captar clientes.',
        tag: 'Web',
        theme: 'theme-teal'
    },
    {
        id: 3,
        title: 'CRM, bot de WhatsApp o app movil',
        description: 'Herramientas para ordenar leads, automatizar atencion y llevar procesos del negocio al celular.',
        tag: 'Sistema',
        theme: 'theme-dark'
    }
]
</script>

<style scoped>
.portfolio-section {
    padding: 82px 24px;
    background: #ffffff;
}

.portfolio-shell {
    max-width: 1180px;
    margin: 0 auto;
}

.portfolio-heading {
    display: grid;
    grid-template-columns: minmax(0, 1fr) auto;
    gap: 24px;
    align-items: end;
    margin-bottom: 34px;
}

.eyebrow {
    display: inline-flex;
    width: fit-content;
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

.portfolio-title {
    max-width: 680px;
    margin: 0;
    color: #12202b;
    font-size: clamp(2rem, 4vw, 3.1rem);
    line-height: 1.08;
}

.portfolio-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0 18px;
    border: 1px solid rgba(18, 32, 43, 0.12);
    border-radius: 8px;
    color: #12202b;
    font-weight: 850;
    text-decoration: none;
}

.portfolio-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}

.portfolio-item {
    overflow: hidden;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background: #ffffff;
    box-shadow: 0 18px 44px rgba(18, 32, 43, 0.07);
}

.portfolio-preview {
    position: relative;
    display: flex;
    align-items: end;
    min-height: 210px;
    padding: 20px;
    overflow: hidden;
}

.portfolio-preview::before {
    content: "";
    position: absolute;
    inset: 24px;
    border: 1px solid rgba(255, 255, 255, 0.22);
    border-radius: 8px;
    background:
        linear-gradient(90deg, rgba(255, 255, 255, 0.12) 1px, transparent 1px),
        linear-gradient(0deg, rgba(255, 255, 255, 0.12) 1px, transparent 1px);
    background-size: 28px 28px;
}

.portfolio-preview span {
    position: relative;
    z-index: 1;
    padding: 8px 11px;
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.18);
    color: #ffffff;
    font-size: 0.78rem;
    font-weight: 850;
    letter-spacing: 0.08em;
    text-transform: uppercase;
}

.theme-blue {
    background: linear-gradient(135deg, #007bff, #18445f);
}

.theme-teal {
    background: linear-gradient(135deg, #00a6a6, #0f3d48);
}

.theme-dark {
    background: linear-gradient(135deg, #12202b, #2b5361);
}

.portfolio-body {
    padding: 24px;
}

.portfolio-item-title {
    margin: 0 0 10px;
    color: #12202b;
    font-size: 1.25rem;
    line-height: 1.25;
}

.portfolio-item-description {
    margin: 0;
    color: #5f6f7b;
    line-height: 1.65;
}

@media (max-width: 900px) {
    .portfolio-heading {
        grid-template-columns: 1fr;
        align-items: start;
    }

    .portfolio-grid {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 640px) {
    .portfolio-section {
        padding: 56px 16px;
    }

    .portfolio-link {
        width: 100%;
    }
}
</style>
