<template>
    <section class="contact-section">
        <div class="contact-shell">
            <div class="form-panel">
                <span class="eyebrow">Contacto directo</span>
                <h2>Hablemos de tu proximo proyecto</h2>
                <p class="intro">
                    Cuentanos que necesitas y te ayudaremos a convertir tu idea en una solucion digital clara,
                    moderna y escalable.
                </p>

                <form class="contact-form" @submit.prevent="submitForm">
                    <div class="field">
                        <label for="name">Nombre completo</label>
                        <input id="name" v-model="name" type="text" placeholder="Ej. Andrea Ramos" required />
                    </div>

                    <div class="field-grid">
                        <div class="field">
                            <label for="email">Correo electronico</label>
                            <input id="email" v-model="email" type="email" placeholder="correo@empresa.com" required />
                        </div>

                        <div class="field">
                            <label for="phone">Telefono</label>
                            <input id="phone" v-model="phone" type="tel" placeholder="+51 999 999 999" />
                        </div>
                    </div>

                    <div class="field">
                        <label for="message">Mensaje</label>
                        <textarea
                            id="message"
                            v-model="message"
                            placeholder="Cuentanos sobre tu proyecto, objetivos o dudas."
                            required
                        ></textarea>
                    </div>

                    <button type="submit" class="submit-button">
                        Enviar mensaje
                    </button>
                </form>
            </div>

            <aside class="tech-panel" aria-label="Fondo tecnologico">
                <div class="tech-grid"></div>
                <div class="signal signal-one"></div>
                <div class="signal signal-two"></div>
                <div class="chip-card">
                    <span>Neurolink</span>
                    <strong>Soluciones digitales inteligentes</strong>
                </div>
                <div class="node node-one"></div>
                <div class="node node-two"></div>
                <div class="node node-three"></div>
            </aside>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            name: '',
            email: '',
            phone: '',
            message: ''
        }
    },
    methods: {
        submitForm() {
            // Ready for integration with a backend or contact service.
        }
    }
}
</script>

<style scoped>
.contact-section {
    min-height: calc(100vh - 74px);
    padding: 64px 24px;
    background:
        radial-gradient(circle at top left, rgba(42, 157, 143, 0.18), transparent 34%),
        linear-gradient(135deg, #eef5f8 0%, #ffffff 48%, #f5f8fb 100%);
}

.contact-shell {
    display: grid;
    grid-template-columns: minmax(0, 0.95fr) minmax(360px, 1.05fr);
    max-width: 1180px;
    min-height: 640px;
    margin: 0 auto;
    overflow: hidden;
    background: rgba(255, 255, 255, 0.82);
    border: 1px solid rgba(20, 36, 48, 0.08);
    border-radius: 8px;
    box-shadow: 0 24px 70px rgba(20, 36, 48, 0.14);
    backdrop-filter: blur(18px);
}

.form-panel {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 56px;
}

.eyebrow {
    width: fit-content;
    margin-bottom: 14px;
    padding: 7px 12px;
    border-radius: 999px;
    background: rgba(0, 123, 255, 0.1);
    color: #0068d9;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
}

h2 {
    max-width: 520px;
    margin: 0;
    color: #12202b;
    font-size: clamp(2rem, 4vw, 3.15rem);
    line-height: 1.05;
}

.intro {
    max-width: 510px;
    margin: 18px 0 32px;
    color: #5f6f7b;
    font-size: 1rem;
    line-height: 1.7;
}

.contact-form {
    display: grid;
    gap: 18px;
}

.field-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 16px;
}

.field {
    display: grid;
    gap: 8px;
}

label {
    color: #1b2c38;
    font-size: 0.88rem;
    font-weight: 700;
}

input,
textarea {
    width: 100%;
    box-sizing: border-box;
    border: 1px solid #dbe4ea;
    border-radius: 8px;
    background: #ffffff;
    color: #142430;
    font: inherit;
    outline: none;
    transition: border-color 0.2s ease, box-shadow 0.2s ease, transform 0.2s ease;
}

input {
    height: 50px;
    padding: 0 16px;
}

textarea {
    min-height: 132px;
    resize: vertical;
    padding: 14px 16px;
}

input:focus,
textarea:focus {
    border-color: #007bff;
    box-shadow: 0 0 0 4px rgba(0, 123, 255, 0.12);
}

.submit-button {
    width: fit-content;
    min-width: 178px;
    height: 52px;
    margin-top: 6px;
    border: 0;
    border-radius: 8px;
    background: linear-gradient(135deg, #007bff, #00a6a6);
    color: #ffffff;
    font-size: 1rem;
    font-weight: 800;
    cursor: pointer;
    box-shadow: 0 16px 32px rgba(0, 123, 255, 0.24);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.submit-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 20px 38px rgba(0, 123, 255, 0.3);
}

.tech-panel {
    position: relative;
    min-height: 520px;
    overflow: hidden;
    background:
        linear-gradient(120deg, rgba(5, 18, 30, 0.92), rgba(11, 61, 84, 0.8)),
        radial-gradient(circle at 30% 20%, rgba(0, 166, 166, 0.8), transparent 36%);
}

.tech-panel::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
        linear-gradient(90deg, rgba(255, 255, 255, 0.07) 1px, transparent 1px),
        linear-gradient(0deg, rgba(255, 255, 255, 0.07) 1px, transparent 1px);
    background-size: 54px 54px;
    mask-image: linear-gradient(90deg, transparent 0%, #000 18%, #000 100%);
}

.tech-grid {
    position: absolute;
    inset: 12%;
    border: 1px solid rgba(119, 235, 255, 0.25);
    border-radius: 8px;
    transform: perspective(900px) rotateX(58deg) rotateZ(-18deg);
    background:
        linear-gradient(90deg, rgba(119, 235, 255, 0.18) 1px, transparent 1px),
        linear-gradient(0deg, rgba(119, 235, 255, 0.18) 1px, transparent 1px);
    background-size: 34px 34px;
    box-shadow: 0 0 80px rgba(0, 166, 166, 0.32);
}

.signal {
    position: absolute;
    height: 2px;
    background: linear-gradient(90deg, transparent, #78f2ff, transparent);
    transform-origin: left center;
    opacity: 0.85;
}

.signal-one {
    width: 62%;
    top: 28%;
    left: 13%;
    transform: rotate(27deg);
}

.signal-two {
    width: 56%;
    right: 8%;
    bottom: 28%;
    transform: rotate(-34deg);
}

.chip-card {
    position: absolute;
    right: 44px;
    bottom: 48px;
    width: min(290px, calc(100% - 88px));
    padding: 24px;
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 8px;
    background: rgba(7, 21, 34, 0.72);
    color: #ffffff;
    box-shadow: 0 24px 50px rgba(0, 0, 0, 0.28);
    backdrop-filter: blur(18px);
}

.chip-card span {
    display: block;
    margin-bottom: 10px;
    color: #78f2ff;
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 0.14em;
    text-transform: uppercase;
}

.chip-card strong {
    display: block;
    font-size: 1.35rem;
    line-height: 1.25;
}

.node {
    position: absolute;
    width: 14px;
    height: 14px;
    border: 3px solid rgba(255, 255, 255, 0.82);
    border-radius: 50%;
    background: #00a6a6;
    box-shadow: 0 0 0 10px rgba(0, 166, 166, 0.18), 0 0 36px rgba(120, 242, 255, 0.8);
}

.node-one {
    top: 24%;
    left: 20%;
}

.node-two {
    top: 47%;
    right: 22%;
}

.node-three {
    left: 35%;
    bottom: 24%;
}

@media (max-width: 900px) {
    .contact-section {
        padding: 32px 16px;
    }

    .contact-shell {
        grid-template-columns: 1fr;
        min-height: auto;
    }

    .form-panel {
        padding: 36px 24px;
    }

    .tech-panel {
        min-height: 320px;
        order: -1;
    }
}

@media (max-width: 640px) {
    .field-grid {
        grid-template-columns: 1fr;
    }

    .submit-button {
        width: 100%;
    }

    .chip-card {
        right: 20px;
        bottom: 20px;
        width: calc(100% - 40px);
    }
}
</style>
