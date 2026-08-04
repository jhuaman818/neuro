<template>
    <section class="pricing-section">
        <div class="pricing-content">
            <h2 class="pricing-title">Planes de Suscripción</h2>
            <p class="pricing-description">Elige el plan que mejor se adapte a tus necesidades y comienza a disfrutar de
                nuestros servicios.</p>
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3 class="card-title">Plan Básico</h3>
                    <p class="card-price">$9.99/mes</p>
                    <ul class="card-features">
                        <li>Acceso limitado a funciones</li>
                        <li>Soporte básico</li>
                    </ul>
                    <button class="card-button">Suscribirse</button>
                </div>
                <div class="pricing-card">
                    <h3 class="card-title">Plan Premium</h3>
                    <p class="card-price">$19.99/mes</p>
                    <ul class="card-features">
                        <li>Acceso completo a todas las funciones</li>
                        <li>Soporte prioritario</li>
                        <li>Actualizaciones exclusivas</li>
                    </ul>
                    <button class="card-button">Suscribirse</button>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.pricing-section {
    padding: 60px 20px;
    background-color: #f9f9f9;
}

.pricing-title {
    font-size: 2rem;
    margin-bottom: 20px;
    text-align: center;
}

.pricing-description {
    font-size: 1.2rem;
    margin-bottom: 40px;
    text-align: center;
    color: #555;
}

.pricing-cards {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.pricing-card {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 300px;
}

.card-title {
    font-size: 1.5rem;
    margin-bottom: 10px;
}

.card-price {
    font-size: 1.25rem;
    margin-bottom: 20px;
    color: #007bff;
}

.card-features {
    list-style: none;
    padding: 0;
    margin-bottom: 20px;
}

.card-button {
    background-color: #007bff;
    color: #fff;
    border: none;
    padding: 10px 20px;
    font-size: 1rem;
    cursor: pointer;
    border-radius: 4px;
}
</style>