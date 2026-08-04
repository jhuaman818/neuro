

<template>
    <div>
        <Navbar />

        <HeroSection />

        <ServicesSection />

        <ProcessSection />

        <TechSection />

        <PortfolioSection />

        <ContactSection />

        <Footer />
    </div>
</template>

<script setup>
import Navbar from '~/components/layout/Navbar.vue'
import HeroSection from '~/components/sections/HeroSection.vue'
import ServicesSection from '~/components/sections/ServicesSection.vue'
import ProcessSection from '~/components/sections/ProcessSection.vue'
import TechSection from '~/components/sections/TechSection.vue'
import PortfolioSection from '~/components/sections/PortfolioSection.vue'
import ContactSection from '~/components/sections/ContactSection.vue'
import Footer from '~/components/layout/Footer.vue'
</script>
