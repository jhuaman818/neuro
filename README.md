# Neurolink

Proyecto web corporativo creado con Nuxt 4, Vue 3 y Tailwind CSS. Es una landing page orientada a presentar servicios, procesos, portafolio, tecnología y contacto.

## Tecnologías

- Nuxt 4
- Vue 3
- Tailwind CSS
- @nuxtjs/tailwindcss
- @nuxt/icon
- @nuxt/fonts
- @vueuse/core
- motion-v

## Características principales

- Diseño responsive desde el primer momento
- Secciones para:
  - Hero
  - Servicios
  - Proceso
  - Portafolio
  - Tecnologías
  - FAQ
  - Contacto
  - Nosotros
- Componentes personalizados reutilizables
- Rutas de páginas para `index`, `servicios`, `portafolio`, `tecnologias`, `nosotros` y `contacto`

## Estructura del proyecto

- `app/` — entrada y plantillas principales de Nuxt
- `app/components/` — componentes y secciones de la UI
- `app/components/sections/` — secciones de la landing
- `app/composables/` — composables personalizados
- `app/layouts/` — layouts compartidos
- `app/pages/` — rutas de la aplicación
- `public/` — archivos estáticos

## Instalación

```bash
npm install
```

## Desarrollo

Inicia el servidor de desarrollo:

```bash
npm run dev
```

Abre `http://localhost:3000` en tu navegador.

## Producción

Construye el proyecto:

```bash
npm run build
```

Previsualiza la versión de producción:

```bash
npm run preview
```

## Recomendaciones

- Asegúrate de revisar `nuxt.config.ts` si necesitas agregar plugins, módulos o ajustes específicos.
- Si vas a desplegar en un hosting estático, usa `npm run generate`.

## Licencia

Licencia no especificada. Agrega una licencia antes de publicar el repositorio si lo deseas.
