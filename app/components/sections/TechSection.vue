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
  { title: 'C#', subtitle: 'Backend .NET', icon: 'logos:csharp' },
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
    position: relative;
    padding: 90px 24px;
    background:
        radial-gradient(circle at 15% 30%, rgba(0, 200, 200, 0.25), transparent 35%),
        radial-gradient(circle at 85% 70%, rgba(0, 123, 255, 0.2), transparent 40%),
        linear-gradient(135deg, #f0fafb 0%, #ffffff 50%, #e8f3f7 100%);
    border-top: 1px solid rgba(0, 200, 200, 0.08);
    border-bottom: 1px solid rgba(0, 123, 255, 0.08);
}

.tech-section::before {
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

.tech-content {
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: minmax(0, 0.95fr) minmax(0, 1.05fr);
    gap: 54px;
    align-items: start;
    max-width: 1280px;
    margin: 0 auto;
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

.tech-title {
    margin: 0;
    color: #08172b;
    font-size: clamp(2rem, 5vw, 3.2rem);
    line-height: 1.1;
    font-weight: 900;
    background: linear-gradient(135deg, #08172b 0%, #0068d9 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.tech-description {
    max-width: 560px;
    margin: 18px 0 0;
    color: #3d4f5c;
    line-height: 1.78;
    font-weight: 500;
}

.tech-stack {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 18px;
}

.tech-card {
    display: grid;
    grid-template-columns: auto 1fr;
    align-items: center;
    gap: 16px;
    min-height: 110px;
    padding: 24px;
    border: 1.5px solid rgba(0, 200, 200, 0.2);
    border-radius: 12px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95), rgba(240, 250, 251, 0.9));
    color: #08172b;
    box-shadow: 0 20px 48px rgba(0, 123, 255, 0.1), inset 0 1px 0 rgba(255, 255, 255, 0.8);
    transition: all 0.3s ease;
}

.tech-card:hover {
    transform: translateY(-6px);
    border-color: rgba(0, 123, 255, 0.3);
    box-shadow: 0 32px 64px rgba(0, 123, 255, 0.18), inset 0 1px 0 rgba(255, 255, 255, 0.8);
}

.tech-card-icon {
    width: 64px;
    height: 64px;
    display: grid;
    place-items: center;
    border-radius: 12px;
    background: linear-gradient(135deg, rgba(0, 123, 255, 0.15), rgba(0, 200, 200, 0.15));
    color: #007bff;
    box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.8), 0 8px 20px rgba(0, 123, 255, 0.12);
    flex-shrink: 0;
}

.tech-card-meta {
    display: grid;
    gap: 6px;
}

.tech-card-title {
    font-size: 1.05rem;
    font-weight: 900;
    line-height: 1.2;
    color: #08172b;
}

.tech-card-meta small {
    color: #3d4f5c;
    font-size: 0.84rem;
    line-height: 1.5;
    font-weight: 500;
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
