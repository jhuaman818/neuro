<template>
    <footer class="footer">
        <div class="footer-inner">
            <div class="footer-brand">
                <span class="brand-mark">N</span>
                <div>
                    <strong>Neurolink</strong>
                    <p>Desarrollo, tecnologia y soluciones digitales para empresas que quieren crecer.</p>
                </div>
            </div>

            <div class="footer-links">
                <NuxtLink to="/servicios">Servicios</NuxtLink>
                <NuxtLink to="/portafolio">Portafolio</NuxtLink>
                <NuxtLink to="/contacto">Contacto</NuxtLink>
            </div>

            <a href="https://wa.me/51935921640" target="_blank" rel="noopener noreferrer" class="footer-cta">
                Escribenos
            </a>
        </div>

        <div class="footer-bottom">
            <span>&copy; {{ new Date().getFullYear() }} Neurolink. Todos los derechos reservados.</span>
        </div>
    </footer>
</template>

<style scoped>
.footer {
    margin-top: 0;
    background:
        radial-gradient(circle at 20% 0%, rgba(0, 166, 166, 0.28), transparent 30%),
        linear-gradient(135deg, #0b1720, #12202b);
    color: #ffffff;
}

.footer-inner {
    display: grid;
    grid-template-columns: 1.2fr auto auto;
    align-items: center;
    gap: 24px;
    max-width: 1180px;
    margin: 0 auto;
    padding: 24px 24px 20px;
}

.footer-brand {
    display: flex;
    align-items: center;
    gap: 16px;
}

.brand-mark {
    display: grid;
    place-items: center;
    width: 46px;
    height: 46px;
    flex: 0 0 auto;
    border-radius: 8px;
    background: linear-gradient(135deg, #007bff, #00a6a6);
    color: #ffffff;
    font-weight: 900;
}

.footer-brand strong {
    display: block;
    margin-bottom: 6px;
    font-size: 1.15rem;
}

.footer-brand p {
    max-width: 460px;
    margin: 0;
    color: rgba(255, 255, 255, 0.68);
    line-height: 1.6;
}

.footer-links {
    display: flex;
    gap: 18px;
}

.footer-links a {
    color: rgba(255, 255, 255, 0.78);
    font-weight: 700;
    text-decoration: none;
    transition: color 0.2s ease;
}

.footer-links a:hover {
    color: #78f2ff;
}

.footer-cta {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 40px;
    padding: 0 16px;
    border: 1px solid rgba(255, 255, 255, 0.22);
    border-radius: 8px;
    color: #ffffff;
    font-weight: 800;
    font-size: 0.92rem;
    text-decoration: none;
    transition: background-color 0.2s ease, transform 0.2s ease;
}

.footer-cta:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-2px);
}

.footer-bottom {
    max-width: 1180px;
    margin: 0 auto;
    padding: 12px 24px 18px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    color: rgba(255, 255, 255, 0.58);
    font-size: 0.88rem;
}

@media (max-width: 820px) {
    .footer-inner {
        grid-template-columns: 1fr;
        align-items: start;
    }

    .footer-links {
        flex-wrap: wrap;
    }
}
</style>
