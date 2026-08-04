<template>
    <section class="faq-section">
        <h2 class="faq-title">Preguntas Frecuentes</h2>
        <div class="faq-list">
            <div class="faq-item" v-for="(faq, index) in faqs" :key="index">
                <h3 class="faq-question">{{ faq.question }}</h3>
                <p class="faq-answer">{{ faq.answer }}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            faqs: [
                { question: '¿Cómo puedo registrarme?', answer: 'Puedes registrarte haciendo clic en el botón de registro en la esquina superior derecha.' },
                { question: '¿Cuál es el costo del servicio?', answer: 'Ofrecemos varios planes, incluyendo uno gratuito. Consulta nuestra página de precios para más detalles.' },
                { question: '¿Puedo cancelar mi suscripción en cualquier momento?', answer: 'Sí, puedes cancelar tu suscripción en cualquier momento desde tu perfil.' },
                { question: '¿Ofrecen soporte técnico?', answer: 'Sí, ofrecemos soporte técnico a través de nuestro chat en vivo y correo electrónico.' }
            ]
        }
    }
}
</script>

<style scoped>
.faq-section {
    padding: 60px 20px;
    background-color: #f9f9f9;
}

.faq-title {
    font-size: 2rem;
    margin-bottom: 40px;
    text-align: center;
}

.faq-list {
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.faq-item {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.faq-question {
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 10px;
}

.faq-answer {
    font-size: 1rem;
    color: #555;
}
</style>
