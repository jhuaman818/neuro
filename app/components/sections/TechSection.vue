<template>
    <section class="tech-section">
        <div class="tech-content">
            <div class="tech-copy">
                <span class="eyebrow">Tecnologia</span>
                <h2 class="tech-title">Tecnologias con las que trabajamos</h2>
                <p class="tech-description">
                    Usamos herramientas probadas para frontend, backend, bases de datos, despliegue y mantenimiento de
                    sistemas en producción.
                </p>
            </div>

            <div class="tech-stack" aria-label="Tecnologias utilizadas">
                <div v-for="item in techItems" :key="item.title" class="tech-card">
                    <div class="tech-card-icon">
                        <Icon :name="item.icon" mode="svg" width="36" height="36" />
                    </div>
                    <div class="tech-card-meta">
                        <span class="tech-card-title">{{ item.title }}</span>
                        <small>{{ item.subtitle }}</small>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
const techItems = [
  { title: 'Vue.js', subtitle: 'Frontend SPA', icon: 'logos:vue' },
  { title: 'Laravel', subtitle: 'Backend PHP moderno', icon: 'simple-icons:laravel' },
  { title: 'PHP', subtitle: 'APIs y CMS', icon: 'logos:php' },
  { title: 'Node.js', subtitle: 'APIs y automatización', icon: 'logos:nodejs-icon' },
  { title: 'Kotlin', subtitle: 'Apps móviles', icon: 'logos:kotlin' },
  { title: 'Docker', subtitle: 'Contenedores', icon: 'logos:docker' },
  { title: 'Laragon', subtitle: 'Entorno local', icon: 'logos:laragon' },
  { title: 'MySQL', subtitle: 'Bases de datos', icon: 'logos:mysql' },
  { title: 'PostgreSQL', subtitle: 'Data con escala', icon: 'logos:postgresql' },
  { title: 'Linux', subtitle: 'Servidores y VPS', icon: 'logos:linux' },
  { title: 'VPS', subtitle: 'Despliegue confiable', icon: 'mdi:server-network' },
  { title: 'Git / GitHub', subtitle: 'Control de versiones', icon: 'logos:github' },
  { title: 'APIs', subtitle: 'Integraciones', icon: 'logos:api' },
  { title: 'WhatsApp', subtitle: 'Automatizaciones', icon: 'logos:whatsapp' },
  { title: 'Y más', subtitle: 'Soluciones a medida', icon: 'mdi:dots-horizontal' }
]
</script>

<style scoped>
.tech-section {
    padding: 78px 24px;
    background: #f5f8fb;
}

.tech-content {
    display: grid;
    grid-template-columns: minmax(0, 0.95fr) minmax(0, 1.05fr);
    gap: 44px;
    align-items: start;
    max-width: 1180px;
    margin: 0 auto;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 14px;
    padding: 8px 14px;
    border-radius: 999px;
    background: rgba(0, 123, 255, 0.1);
    color: #0068d9;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.1em;
    text-transform: uppercase;
}

.tech-title {
    margin: 0;
    color: #12202b;
    font-size: clamp(2rem, 4vw, 3rem);
    line-height: 1.08;
}

.tech-description {
    max-width: 560px;
    margin: 18px 0 0;
    color: #5f6f7b;
    line-height: 1.72;
}

.tech-stack {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
    gap: 16px;
}

.tech-card {
    display: grid;
    grid-template-columns: auto 1fr;
    align-items: center;
    gap: 14px;
    min-height: 100px;
    padding: 22px 22px;
    border: 1px solid rgba(18, 32, 43, 0.08);
    border-radius: 22px;
    background: linear-gradient(180deg, #ffffff 0%, #f7fafe 100%);
    color: #12202b;
    box-shadow: 0 26px 58px rgba(18, 32, 43, 0.08);
    transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.tech-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 32px 64px rgba(18, 32, 43, 0.14);
}

.tech-card-icon {
    width: 58px;
    height: 58px;
    display: grid;
    place-items: center;
    border-radius: 18px;
    background: linear-gradient(180deg, rgba(0, 123, 255, 0.16), rgba(0, 123, 255, 0.04));
    color: #0068d9;
    box-shadow: inset 0 1px 0 rgba(255,255,255,0.8), 0 8px 16px rgba(0, 123, 255, 0.08);
}

.tech-card-meta {
    display: grid;
    gap: 6px;
}

.tech-card-title {
    font-size: 1rem;
    font-weight: 850;
    line-height: 1.2;
}

.tech-card-meta small {
    color: #5f6f7b;
    font-size: 0.85rem;
    line-height: 1.5;
}

@media (max-width: 980px) {
    .tech-content {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 820px) {
    .tech-stack {
        grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
    }
}

@media (max-width: 640px) {
    .tech-section {
        padding: 56px 16px;
    }

    .tech-card {
        grid-template-columns: 1fr;
        text-align: center;
    }

    .tech-card-icon {
        margin: 0 auto;
    }
}
</style>
