<template>
    <header class="site-header">
        <nav class="navbar" aria-label="Navegacion principal">
            <NuxtLink to="/" class="brand" aria-label="Neurolink inicio">
                <span class="brand-mark">N</span>
                <span class="brand-text">Neurolink</span>
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

<style lang="css" scoped>
.site-header {
    position: sticky;
    top: 0;
    z-index: 20;
    border-bottom: 1px solid rgba(18, 32, 43, 0.08);
    background: rgba(255, 255, 255, 0.88);
    backdrop-filter: blur(18px);
}

.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1180px;
    min-height: 74px;
    margin: 0 auto;
    padding: 0 24px;
    gap: 28px;
}

.brand {
    display: inline-flex;
    align-items: center;
    gap: 11px;
    color: #12202b;
    text-decoration: none;
}

.brand-mark {
    display: grid;
    place-items: center;
    width: 42px;
    height: 42px;
    border-radius: 8px;
    background:
        linear-gradient(135deg, rgba(0, 123, 255, 0.95), rgba(0, 166, 166, 0.95)),
        #007bff;
    color: #ffffff;
    font-weight: 900;
    box-shadow: 0 14px 28px rgba(0, 123, 255, 0.22);
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
    padding: 10px 12px;
    border-radius: 8px;
    color: #435461;
    font-size: 0.94rem;
    font-weight: 700;
    text-decoration: none;
    transition: color 0.2s ease, background-color 0.2s ease;
}

.navbar-menu a:hover,
.navbar-menu a.router-link-active {
    background: rgba(0, 123, 255, 0.08);
    color: #0068d9;
}

.quote-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 44px;
    padding: 0 18px;
    border-radius: 8px;
    background: #12202b;
    color: #ffffff;
    font-size: 0.92rem;
    font-weight: 800;
    text-decoration: none;
    box-shadow: 0 14px 30px rgba(18, 32, 43, 0.18);
    transition: transform 0.2s ease, background-color 0.2s ease, box-shadow 0.2s ease;
    white-space: nowrap;
}

.quote-button:hover {
    transform: translateY(-2px);
    background: #007bff;
    box-shadow: 0 18px 36px rgba(0, 123, 255, 0.25);
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
