<script setup lang="ts">
import Navbar from '~/components/layout/Navbar.vue'
import Footer from '~/components/layout/Footer.vue'

const projectTypes = [
    {
        title: 'Correccion de facturacion electronica',
        category: 'Soporte tecnico',
        description:
            'Revision y solucion de errores en sistemas de facturacion, documentos electronicos, reportes, integraciones y flujos criticos.',
        technologies: ['PHP', 'Laravel', 'MySQL', 'APIs'],
        result: 'Sistema mas estable y procesos de emision funcionando correctamente.',
        accent: 'blue'
    },
    {
        title: 'Pagina web corporativa',
        category: 'Presencia digital',
        description:
            'Sitios web modernos para empresas, profesionales y negocios que necesitan presentar servicios, recibir consultas y generar confianza.',
        technologies: ['Vue.js', 'Laravel', 'Node.js', 'SEO'],
        result: 'Marca mejor presentada, contacto directo por WhatsApp y estructura responsive.',
        accent: 'teal'
    },
    {
        title: 'Landing page de ventas',
        category: 'Conversion',
        description:
            'Paginas enfocadas en campanas, promociones, cursos, productos o servicios con formularios, botones de accion y mensajes claros.',
        technologies: ['Vue.js', 'PHP', 'GitHub', 'VPS'],
        result: 'Mayor captacion de leads y una pagina lista para anuncios o redes sociales.',
        accent: 'dark'
    },
    {
        title: 'CRM para gestion comercial',
        category: 'Sistema interno',
        description:
            'Paneles para ordenar clientes, oportunidades, estados, tareas, vendedores y seguimiento comercial desde un solo lugar.',
        technologies: ['Laravel', 'Node.js', 'PostgreSQL', 'Docker'],
        result: 'Ventas mas ordenadas, informacion centralizada y seguimiento claro de clientes.',
        accent: 'blue'
    },
    {
        title: 'Bot de WhatsApp',
        category: 'Automatizacion',
        description:
            'Flujos para responder consultas, capturar datos, derivar clientes, enviar avisos y conectar WhatsApp con sistemas internos.',
        technologies: ['Node.js', 'APIs', 'Linux', 'VPS'],
        result: 'Atencion mas rapida y menos consultas perdidas fuera del horario de trabajo.',
        accent: 'teal'
    },
    {
        title: 'Aplicacion movil',
        category: 'Movil',
        description:
            'Apps para negocios, reservas, reportes, pedidos, notificaciones o herramientas internas conectadas a backend y base de datos.',
        technologies: ['Kotlin', 'Laravel', 'MySQL', 'Git'],
        result: 'Procesos disponibles desde el celular para clientes, equipos o administradores.',
        accent: 'dark'
    }
]

const workflow = [
    'Analizamos la necesidad o el sistema actual',
    'Definimos alcance, prioridades y tecnologias',
    'Desarrollamos, corregimos o integramos por etapas',
    'Probamos, publicamos y dejamos soporte listo'
]
</script>

<template>
    <div>
        <Navbar />

        <main>
            <section class="portfolio-hero">
                <div class="hero-inner">
                    <div class="hero-copy">
                        <span class="eyebrow">Portafolio</span>
                        <h1>Soluciones que podemos desarrollar para tu negocio</h1>
                        <p>
                            Estos son los tipos de proyectos que trabajamos en Neurolink: correcciones de sistemas,
                            paginas web, landing pages, CRM, bots de WhatsApp, automatizaciones y aplicaciones moviles.
                        </p>
                        <div class="hero-actions">
                            <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="primary-action">
                                Solicitar proyecto similar
                            </a>
                            <NuxtLink to="/contacto" class="secondary-action">Enviar consulta</NuxtLink>
                        </div>
                    </div>

                    <aside class="hero-panel" aria-label="Resumen de portafolio">
                        <div class="panel-header">
                            <span>Neurolink</span>
                            <strong>Stack operativo</strong>
                        </div>
                        <div class="panel-grid">
                            <span>Vue.js</span>
                            <span>Laravel</span>
                            <span>Node.js</span>
                            <span>Kotlin</span>
                            <span>Docker</span>
                            <span>VPS</span>
                        </div>
                    </aside>
                </div>
            </section>

            <section class="projects-section">
                <div class="section-heading">
                    <span class="eyebrow">Casos tipo</span>
                    <h2>Proyectos organizados por necesidad</h2>
                    <p>
                        Cada tarjeta muestra que se puede construir, corregir o automatizar. Cuando tengas casos reales
                        con cliente, esta misma estructura se puede convertir en portafolio con capturas y enlaces.
                    </p>
                </div>

                <div class="projects-grid">
                    <article
                        v-for="project in projectTypes"
                        :key="project.title"
                        class="project-card"
                        :class="`accent-${project.accent}`"
                    >
                        <div class="project-preview">
                            <span>{{ project.category }}</span>
                        </div>
                        <div class="project-body">
                            <h3>{{ project.title }}</h3>
                            <p>{{ project.description }}</p>

                            <div class="tech-list" aria-label="Tecnologias">
                                <span v-for="tech in project.technologies" :key="tech">{{ tech }}</span>
                            </div>

                            <div class="result-box">
                                <strong>Resultado esperado</strong>
                                <p>{{ project.result }}</p>
                            </div>
                        </div>
                    </article>
                </div>
            </section>

            <section class="workflow-section">
                <div class="workflow-inner">
                    <div>
                        <span class="eyebrow">Proceso</span>
                        <h2>Como llevamos un proyecto desde la idea hasta produccion</h2>
                    </div>

                    <div class="workflow-list">
                        <div v-for="(step, index) in workflow" :key="step" class="workflow-item">
                            <span>{{ String(index + 1).padStart(2, '0') }}</span>
                            <p>{{ step }}</p>
                        </div>
                    </div>
                </div>
            </section>

            <section class="cta-section">
                <div class="cta-inner">
                    <span class="eyebrow">Cotizacion</span>
                    <h2>Necesitas algo parecido?</h2>
                    <p>
                        Podemos revisar tu sistema actual, corregir errores o crear una solucion nueva segun el objetivo
                        de tu negocio.
                    </p>
                    <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="primary-action">
                        Escribir por WhatsApp
                    </a>
                </div>
            </section>
        </main>

        <Footer />
    </div>
</template>

<style scoped>
main {
    background: #ffffff;
}

.portfolio-hero {
    position: relative;
    overflow: hidden;
    padding: 82px 24px 72px;
    background:
        radial-gradient(circle at 12% 14%, rgba(0, 166, 166, 0.18), transparent 30%),
        radial-gradient(circle at 88% 6%, rgba(0, 123, 255, 0.16), transparent 28%),
        linear-gradient(135deg, #f5fbfc 0%, #ffffff 48%, #eef5f8 100%);
}

.portfolio-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(18, 32, 43, 0.045) 1px, transparent 1px),
        linear-gradient(0deg, rgba(18, 32, 43, 0.045) 1px, transparent 1px);
    background-size: 54px 54px;
    mask-image: linear-gradient(180deg, #000 0%, transparent 82%);
}

.hero-inner,
.workflow-inner,
.cta-inner,
.projects-section {
    max-width: 1180px;
    margin: 0 auto;
}

.hero-inner {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 1fr) minmax(340px, 0.72fr);
    gap: 48px;
    align-items: center;
}

.hero-copy {
    max-width: 760px;
}

.eyebrow {
    display: inline-flex;
    width: fit-content;
    margin-bottom: 14px;
    padding: 7px 12px;
    border-radius: 999px;
    background: rgba(0, 123, 255, 0.1);
    color: #0068d9;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.1em;
    text-transform: uppercase;
}

h1,
h2,
h3,
p {
    margin: 0;
}

h1 {
    color: #12202b;
    font-size: clamp(2.45rem, 5vw, 4.7rem);
    line-height: 1;
}

.hero-copy p,
.section-heading p,
.cta-inner p {
    color: #5f6f7b;
    line-height: 1.75;
}

.hero-copy > p {
    max-width: 690px;
    margin-top: 22px;
    font-size: 1.08rem;
}

.hero-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
    margin-top: 32px;
}

.primary-action,
.secondary-action {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 50px;
    padding: 0 20px;
    border-radius: 8px;
    font-weight: 850;
    text-decoration: none;
}

.primary-action {
    background: linear-gradient(135deg, #007bff, #00a6a6);
    color: #ffffff;
    box-shadow: 0 18px 36px rgba(0, 123, 255, 0.24);
}

.secondary-action {
    border: 1px solid rgba(18, 32, 43, 0.12);
    background: rgba(255, 255, 255, 0.82);
    color: #12202b;
}

.hero-panel {
    padding: 26px;
    border-radius: 8px;
    background:
        linear-gradient(145deg, rgba(8, 22, 34, 0.94), rgba(13, 74, 94, 0.86)),
        #12202b;
    color: #ffffff;
    box-shadow: 0 34px 80px rgba(18, 32, 43, 0.24);
}

.panel-header {
    display: flex;
    justify-content: space-between;
    gap: 16px;
    margin-bottom: 22px;
}

.panel-header span {
    color: #78f2ff;
    font-weight: 850;
}

.panel-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 12px;
}

.panel-grid span {
    display: grid;
    place-items: center;
    min-height: 72px;
    border: 1px solid rgba(255, 255, 255, 0.12);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.08);
    color: rgba(255, 255, 255, 0.88);
    font-weight: 800;
}

.projects-section {
    padding: 82px 24px;
}

.section-heading {
    max-width: 780px;
    margin-bottom: 38px;
}

.section-heading h2,
.workflow-inner h2,
.cta-inner h2 {
    color: #12202b;
    font-size: clamp(2rem, 4vw, 3.15rem);
    line-height: 1.08;
}

.section-heading p {
    margin-top: 16px;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}

.project-card {
    overflow: hidden;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background: #ffffff;
    box-shadow: 0 18px 44px rgba(18, 32, 43, 0.07);
}

.project-preview {
    position: relative;
    display: flex;
    align-items: end;
    min-height: 160px;
    padding: 20px;
    overflow: hidden;
}

.project-preview::before {
    content: "";
    position: absolute;
    inset: 22px;
    border: 1px solid rgba(255, 255, 255, 0.22);
    border-radius: 8px;
    background:
        linear-gradient(90deg, rgba(255, 255, 255, 0.12) 1px, transparent 1px),
        linear-gradient(0deg, rgba(255, 255, 255, 0.12) 1px, transparent 1px);
    background-size: 28px 28px;
}

.project-preview span {
    position: relative;
    z-index: 1;
    padding: 8px 11px;
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.18);
    color: #ffffff;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.08em;
    text-transform: uppercase;
}

.accent-blue .project-preview {
    background: linear-gradient(135deg, #007bff, #18445f);
}

.accent-teal .project-preview {
    background: linear-gradient(135deg, #00a6a6, #0f3d48);
}

.accent-dark .project-preview {
    background: linear-gradient(135deg, #12202b, #2b5361);
}

.project-body {
    display: grid;
    gap: 16px;
    padding: 24px;
}

.project-body h3 {
    color: #12202b;
    font-size: 1.24rem;
    line-height: 1.25;
}

.project-body > p,
.result-box p {
    color: #5f6f7b;
    line-height: 1.65;
}

.tech-list {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
}

.tech-list span {
    padding: 7px 10px;
    border-radius: 999px;
    background: #f0f6f8;
    color: #1d3442;
    font-size: 0.82rem;
    font-weight: 800;
}

.result-box {
    padding: 16px;
    border-radius: 8px;
    background: #f7fafb;
}

.result-box strong {
    display: block;
    margin-bottom: 8px;
    color: #12202b;
    font-size: 0.9rem;
}

.workflow-section {
    padding: 76px 24px;
    background: linear-gradient(135deg, #0b1720, #12202b);
    color: #ffffff;
}

.workflow-inner {
    display: grid;
    grid-template-columns: minmax(0, 0.86fr) minmax(0, 1.14fr);
    gap: 44px;
    align-items: start;
}

.workflow-section .eyebrow {
    background: rgba(120, 242, 255, 0.12);
    color: #78f2ff;
}

.workflow-inner h2 {
    color: #ffffff;
}

.workflow-list {
    display: grid;
    gap: 14px;
}

.workflow-item {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 16px;
    align-items: center;
    padding: 20px;
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.06);
}

.workflow-item span {
    color: #78f2ff;
    font-weight: 900;
}

.workflow-item p {
    color: rgba(255, 255, 255, 0.76);
    line-height: 1.55;
}

.cta-section {
    padding: 78px 24px;
    background: #f5f8fb;
}

.cta-inner {
    padding: 42px;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 8px;
    background: #ffffff;
    box-shadow: 0 18px 44px rgba(18, 32, 43, 0.07);
}

.cta-inner p {
    max-width: 650px;
    margin: 16px 0 26px;
}

@media (max-width: 960px) {
    .hero-inner,
    .workflow-inner {
        grid-template-columns: 1fr;
    }

    .projects-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }
}

@media (max-width: 640px) {
    .portfolio-hero,
    .projects-section,
    .workflow-section,
    .cta-section {
        padding-left: 16px;
        padding-right: 16px;
    }

    .projects-grid,
    .panel-grid {
        grid-template-columns: 1fr;
    }

    .hero-actions,
    .primary-action,
    .secondary-action {
        width: 100%;
    }

    .cta-inner {
        padding: 28px 20px;
    }
}
</style>
