<template>
    <header class="site-header">
        <nav class="navbar" aria-label="Navegacion principal">
            <NuxtLink to="/" class="brand" aria-label="Neurolink inicio">
                <img :src="logo" alt="Neurolink logo" class="brand-mark" />
                <!-- <span class="brand-text">Neurolink</span> -->
            </NuxtLink>

            <div class="navbar-menu">
                <NuxtLink to="/">Inicio</NuxtLink>
                <NuxtLink to="/servicios">Servicios</NuxtLink>
                <NuxtLink to="/portafolio">Portafolio</NuxtLink>
                <NuxtLink to="/tecnologias">Tecnologias</NuxtLink>
                <NuxtLink to="/nosotros">Nosotros</NuxtLink>
                <NuxtLink to="/contacto">Contacto</NuxtLink>
            </div>

            <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="quote-button">
                Solicitar cotizacion
            </a>
        </nav>
    </header>
</template>

<script setup lang="ts">
import logo from '~/assets/images/logo .png'
</script>

<style lang="css" scoped>
.site-header {
    position: sticky;
    top: 0;
    z-index: 20;
    border-bottom: 1px solid rgba(0, 200, 200, 0.15);
    background: linear-gradient(135deg, rgba(8, 25, 40, 0.92), rgba(10, 40, 60, 0.92));
    backdrop-filter: blur(20px);
    box-shadow: 0 4px 24px rgba(0, 123, 255, 0.08);
}

.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1280px;
    min-height: 90px;
    margin: 0 auto;
    padding: 10px 24px;
    gap: 28px;
}

.brand {
    display: inline-flex;
    align-items: center;
    gap: 11px;
    color: #ffffff;
    text-decoration: none;
}

.brand-mark {
    display: block;
    width: 160px;
    height: auto;
    object-fit: contain;
    border-radius: 0;
    box-shadow: none;
}

.brand-text {
    font-size: 1.12rem;
    font-weight: 900;
}

.navbar-menu {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 6px;
    flex: 1;
}

.navbar-menu a {
    position: relative;
    padding: 10px 14px;
    border-radius: 8px;
    color: rgba(255, 255, 255, 0.75);
    font-size: 0.94rem;
    font-weight: 700;
    text-decoration: none;
    transition: color 0.2s ease, background-color 0.2s ease;
}

.navbar-menu a:hover,
.navbar-menu a.router-link-active {
    background: rgba(0, 200, 200, 0.15);
    color: #00d4ff;
}

.quote-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 48px;
    padding: 0 22px;
    border-radius: 8px;
    background: linear-gradient(135deg, #007bff, #0a5fc4);
    color: #ffffff;
    font-size: 0.92rem;
    font-weight: 900;
    text-decoration: none;
    box-shadow: 0 16px 40px rgba(0, 123, 255, 0.3);
    transition: all 0.3s ease;
    white-space: nowrap;
}

.quote-button:hover {
    transform: translateY(-2px);
    background: linear-gradient(135deg, #0090ff, #1575ff);
    box-shadow: 0 24px 48px rgba(0, 123, 255, 0.4);
}

@media (max-width: 960px) {
    .navbar {
        flex-wrap: wrap;
        padding: 14px 18px;
        gap: 14px;
    }

    .navbar-menu {
        order: 3;
        flex-basis: 100%;
        justify-content: flex-start;
        overflow-x: auto;
        padding-bottom: 2px;
    }
}

@media (max-width: 560px) {
    .brand-text {
        font-size: 1rem;
    }

    .quote-button {
        min-height: 40px;
        padding: 0 13px;
        font-size: 0.82rem;
    }
}
</style>
