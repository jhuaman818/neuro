<script setup lang="ts">
import Footer from '~/components/layout/Footer.vue';
import Navbar from '~/components/layout/Navbar.vue';
import NosotrosSection from '~/components/sections/Nosotros.vue';
</script>

<template>
    <Navbar />

    <NosotrosSection />

    <Footer />
</template>
<style scoped>
.about-page {
    max-width: 1180px;
    margin: 0 auto;
    padding: 80px 24px 48px;
    display: grid;
    gap: 36px;
}

.about-hero {
    max-width: 730px;
}

.eyebrow {
    display: inline-flex;
    margin-bottom: 16px;
    padding: 7px 14px;
    border-radius: 999px;
    background: rgba(0, 123, 255, 0.1);
    color: #0068d9;
    font-size: 0.76rem;
    font-weight: 850;
    letter-spacing: 0.12em;
    text-transform: uppercase;
}

.about-hero h1 {
    margin: 0;
    color: #12202b;
    font-size: clamp(2.4rem, 4vw, 3.6rem);
    line-height: 1.02;
}

.about-hero p {
    max-width: 620px;
    margin: 18px 0 0;
    color: #556471;
    font-size: 1rem;
    line-height: 1.8;
}

.about-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}

.about-card {
    padding: 28px 26px;
    border-radius: 24px;
    background: linear-gradient(180deg, #ffffff 0%, #f7fafd 100%);
    border: 1px solid rgba(18, 32, 43, 0.08);
    box-shadow: 0 18px 38px rgba(18, 32, 43, 0.06);
}

.about-card h2 {
    margin: 0 0 14px;
    font-size: 1.2rem;
    color: #12202b;
}

.about-card p {
    margin: 0;
    color: #5f6f7b;
    line-height: 1.75;
}

.about-extra {
    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    gap: 20px;
}

.about-extra-card {
    padding: 28px 30px;
    border-radius: 24px;
    background: #f1f7fb;
    border: 1px solid rgba(0, 123, 255, 0.12);
}

.about-extra-card h3 {
    margin: 0 0 14px;
    color: #12202b;
    font-size: 1.15rem;
}

.about-extra-card p,
.about-extra-card ul {
    margin: 0;
    color: #5f6f7b;
    line-height: 1.75;
}

.about-extra-card ul {
    padding-left: 18px;
}

.about-extra-card li {
    margin-bottom: 10px;
}

.about-cta {
    display: grid;
    grid-template-columns: minmax(0, 1fr) auto;
    align-items: center;
    gap: 24px;
    padding: 28px 30px;
    border-radius: 24px;
    background: linear-gradient(135deg, #eaf6ff, #f8fbff);
    border: 1px solid rgba(0, 123, 255, 0.14);
}

.about-cta p {
    margin: 0;
    color: #12202b;
    font-size: 1rem;
    line-height: 1.8;
}

.button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 48px;
    padding: 0 22px;
    border-radius: 12px;
    background: #12202b;
    color: #ffffff;
    font-weight: 800;
    text-decoration: none;
    transition: transform 0.2s ease, background-color 0.2s ease;
}

.button:hover {
    transform: translateY(-2px);
    background: #007bff;
}

@media (max-width: 980px) {
    .about-grid,
    .about-extra,
    .about-cta {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 640px) {
    .about-page {
        padding: 56px 18px 36px;
    }

    .about-card,
    .about-extra-card,
    .about-cta {
        padding: 22px;
    }
}
</style>