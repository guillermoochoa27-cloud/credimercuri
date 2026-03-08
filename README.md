# credimercuri
SERVICIOS FINACIEROS
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Credimercuri - Préstamos Personales en Villa Dolores | Encuesta</title>
<meta name="description" content="Préstamos personales en 24hs para jubilados, pensionados, pensiones no contributivas y empleados en Villa Dolores, Córdoba. Hipólito Yrigoyen 655.">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
<style>
* {
margin: 0;
padding: 0;
box-sizing: border-box;
}

:root {
--primary: #1a237e;
--primary-dark: #0d1642;
--secondary: #00bfa5;
--accent: #ffd600;
--whatsapp: #25d366;
--whatsapp-dark: #128c7e;
--urgent: #ff5722;
--text: #333333;
--text-light: #666666;
--bg: #f8f9fa;
--white: #ffffff;
--shadow: 0 4px 20px rgba(0,0,0,0.1);
--shadow-strong: 0 8px 40px rgba(0,0,0,0.15);
}

html {
scroll-behavior: smooth;
}

body {
font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
background: var(--white);
color: var(--text);
line-height: 1.6;
overflow-x: hidden;
}

/* Header */
.header {
background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
color: var(--white);
padding: 16px 0;
position: fixed;
width: 100%;
top: 0;
z-index: 1000;
box-shadow: var(--shadow);
}

.header-content {
max-width: 1200px;
margin: 0 auto;
padding: 0 20px;
display: flex;
justify-content: space-between;
align-items: center;
}

.logo {
display: flex;
align-items: center;
gap: 12px;
font-size: 24px;
font-weight: 800;
}

.logo-icon {
width: 48px;
height: 48px;
background: var(--accent);
border-radius: 12px;
display: flex;
align-items: center;
justify-content: center;
font-size: 28px;
}

.header-contact {
display: flex;
align-items: center;
gap: 20px;
}

.header-whatsapp {
background: var(--whatsapp);
color: var(--white);
padding: 12px 24px;
border-radius: 50px;
text-decoration: none;
font-weight: 700;
display: flex;
align-items: center;
gap: 8px;
transition: all 0.3s;
box-shadow: 0 4px 15px rgba(37,211,102,0.4);
}

.header-whatsapp:hover {
transform: translateY(-2px);
box-shadow: 0 6px 20px rgba(37,211,102,0.6);
}

.menu-toggle {
display: none;
font-size: 28px;
cursor: pointer;
}

/* Hero Section */
.hero {
background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 50%, var(--secondary) 100%);
color: var(--white);
padding: 140px 20px 80px;
position: relative;
overflow: hidden;
}

.hero::before {
content: '';
position: absolute;
top: 0;
left: 0;
right: 0;
bottom: 0;
background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="%23ffffff" fill-opacity="0.05" d="M0,96L48,112C96,128,192,160,288,186.7C384,213,480,235,576,213.3C672,192,768,128,864,128C960,128,1056,192,1152,208C1248,224,1344,192,1392,176L1440,160L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
background-size: cover;
opacity: 0.3;
}

.hero-content {
max-width: 1200px;
margin: 0 auto;
position: relative;
z-index: 2;
text-align: center;
}

.hero-text h1 {
font-size: 52px;
font-weight: 800;
line-height: 1.2;
margin-bottom: 24px;
}

.hero-text h1 span {
color: var(--accent);
}

.hero-subtitle {
font-size: 20px;
opacity: 0.95;
margin-bottom: 32px;
line-height: 1.6;
max-width: 700px;
margin-left: auto;
margin-right: auto;
}

.hero-features {
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 24px;
margin-bottom: 40px;
}

.hero-feature {
display: flex;
align-items: center;
gap: 12px;
font-size: 16px;
background: rgba(255,255,255,0.1);
padding: 12px 20px;
border-radius: 50px;
backdrop-filter: blur(10px);
}

.hero-feature-icon {
width: 32px;
height: 32px;
background: var(--accent);
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
font-size: 16px;
flex-shrink: 0;
}

/* SURVEY SECTION - NUEVA */
.survey-section {
padding: 60px 20px;
background: var(--bg);
}

.survey-container {
max-width: 800px;
margin: 0 auto;
background: var(--white);
border-radius: 24px;
padding: 40px;
box-shadow: var(--shadow-strong);
border: 2px solid var(--secondary);
}

.survey-header {
text-align: center;
margin-bottom: 40px;
}

.survey-header h2 {
font-size: 32px;
color: var(--primary);
margin-bottom: 12px;
}

.survey-header p {
color: var(--text-light);
font-size: 16px;
}

.survey-progress {
display: flex;
justify-content: center;
gap: 8px;
margin-bottom: 40px;
}

.progress-dot {
width: 12px;
height: 12px;
border-radius: 50%;
background: #e0e0e0;
transition: all 0.3s;
}

.progress-dot.active {
background: var(--secondary);
transform: scale(1.2);
}

.progress-dot.completed {
background: var(--whatsapp);
}

.survey-step {
display: none;
}

.survey-step.active {
display: block;
animation: fadeIn 0.5s;
}

@keyframes fadeIn {
from { opacity: 0; transform: translateY(20px); }
to { opacity: 1; transform: translateY(0); }
}

.question-title {
font-size: 24px;
font-weight: 700;
color: var(--primary);
margin-bottom: 24px;
text-align: center;
}

.question-subtitle {
font-size: 16px;
color: var(--text-light);
margin-bottom: 32px;
text-align: center;
}

.options-grid {
display: grid;
grid-template-columns: repeat(2, 1fr);
gap: 16px;
margin-bottom: 32px;
}

.option-card {
background: var(--bg);
border: 2px solid transparent;
border-radius: 16px;
padding: 24px;
cursor: pointer;
transition: all 0.3s;
text-align: center;
}

.option-card:hover {
border-color: var(--secondary);
transform: translateY(-4px);
box-shadow: var(--shadow);
}

.option-card.selected {
background: linear-gradient(135deg, var(--primary), var(--secondary));
color: white;
border-color: var(--primary);
}

.option-icon {
font-size: 40px;
margin-bottom: 12px;
}

.option-label {
font-size: 16px;
font-weight: 600;
}

.option-hint {
font-size: 13px;
opacity: 0.8;
margin-top: 4px;
}

.input-group {
margin-bottom: 24px;
}

.input-group label {
display: block;
font-weight: 600;
color: var(--primary);
margin-bottom: 8px;
font-size: 16px;
}

.input-group input,
.input-group select {
width: 100%;
padding: 16px;
border: 2px solid #e0e0e0;
border-radius: 12px;
font-size: 16px;
transition: border-color 0.3s;
font-family: inherit;
}

.input-group input:focus,
.input-group select:focus {
outline: none;
border-color: var(--secondary);
}

.input-hint {
font-size: 13px;
color: var(--text-light);
margin-top: 6px;
}

.amount-display {
background: linear-gradient(135deg, var(--accent), #ffecb3);
color: var(--primary-dark);
padding: 20px;
border-radius: 16px;
text-align: center;
margin: 24px 0;
}

.amount-display h4 {
font-size: 14px;
margin-bottom: 8px;
opacity: 0.9;
}

.amount-display .amount {
font-size: 36px;
font-weight: 800;
}

.survey-buttons {
display: flex;
gap: 16px;
justify-content: center;
margin-top: 32px;
}

.btn-survey {
padding: 16px 32px;
border-radius: 12px;
border: none;
font-size: 16px;
font-weight: 700;
cursor: pointer;
transition: all 0.3s;
display: flex;
align-items: center;
gap: 8px;
}

.btn-primary {
background: var(--primary);
color: white;
}

.btn-primary:hover:not(:disabled) {
background: var(--primary-dark);
transform: translateY(-2px);
}

.btn-primary:disabled {
opacity: 0.5;
cursor: not-allowed;
}

.btn-secondary {
background: var(--bg);
color: var(--text);
}

.btn-secondary:hover {
background: #e0e0e0;
}

.btn-whatsapp {
background: var(--whatsapp);
color: white;
font-size: 18px;
padding: 20px 40px;
animation: pulse-whatsapp 2s infinite;
}

@keyframes pulse-whatsapp {
0%, 100% { transform: scale(1); box-shadow: 0 4px 20px rgba(37,211,102,0.4); }
50% { transform: scale(1.02); box-shadow: 0 6px 30px rgba(37,211,102,0.6); }
}

.summary-box {
background: linear-gradient(135deg, #f5f5f5, #fafafa);
border-radius: 16px;
padding: 24px;
margin-bottom: 24px;
}

.summary-item {
display: flex;
justify-content: space-between;
padding: 12px 0;
border-bottom: 1px solid #e0e0e0;
}

.summary-item:last-child {
border-bottom: none;
}

.summary-label {
color: var(--text-light);
font-size: 14px;
}

.summary-value {
font-weight: 700;
color: var(--primary);
font-size: 14px;
}

.eligibility-badge {
display: inline-block;
padding: 12px 24px;
border-radius: 50px;
font-weight: 700;
font-size: 16px;
margin-bottom: 24px;
}

.eligible {
background: linear-gradient(135deg, #4caf50, #45a049);
color: white;
}

.review {
background: linear-gradient(135deg, #ff9800, #f57c00);
color: white;
}

/* Services Section */
.services {
padding: 80px 20px;
background: var(--white);
}

.container {
max-width: 1200px;
margin: 0 auto;
}

.section-header {
text-align: center;
margin-bottom: 60px;
}

.section-header h2 {
font-size: 40px;
font-weight: 800;
color: var(--primary);
margin-bottom: 16px;
}

.section-header p {
font-size: 18px;
color: var(--text-light);
max-width: 600px;
margin: 0 auto;
}

.services-grid {
display: grid;
grid-template-columns: repeat(4, 1fr);
gap: 24px;
}

.service-card {
background: var(--bg);
border-radius: 20px;
padding: 32px;
text-align: center;
transition: all 0.3s;
border: 2px solid transparent;
}

.service-card:hover {
transform: translateY(-8px);
box-shadow: var(--shadow-strong);
border-color: var(--secondary);
}

.service-icon {
width: 80px;
height: 80px;
background: linear-gradient(135deg, var(--primary), var(--secondary));
border-radius: 20px;
display: flex;
align-items: center;
justify-content: center;
font-size: 40px;
margin: 0 auto 20px;
}

.service-card h3 {
font-size: 20px;
font-weight: 700;
margin-bottom: 12px;
color: var(--primary);
}

.service-card p {
font-size: 15px;
color: var(--text-light);
line-height: 1.6;
}

/* Process Section */
.process {
padding: 80px 20px;
background: var(--bg);
}

.process-steps {
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 40px;
margin-top: 60px;
}

.process-step {
text-align: center;
position: relative;
}

.process-step:not(:last-child)::after {
content: '→';
position: absolute;
top: 40px;
right: -30px;
font-size: 40px;
color: var(--secondary);
font-weight: 700;
}

.step-number {
width: 80px;
height: 80px;
background: linear-gradient(135deg, var(--primary), var(--secondary));
color: var(--white);
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
font-size: 32px;
font-weight: 800;
margin: 0 auto 24px;
box-shadow: 0 8px 20px rgba(26,35,126,0.3);
}

.process-step h3 {
font-size: 22px;
font-weight: 700;
margin-bottom: 12px;
color: var(--primary);
}

.process-step p {
font-size: 16px;
color: var(--text-light);
}

/* Testimonials */
.testimonials {
padding: 80px 20px;
background: var(--white);
}

.testimonials-grid {
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 24px;
margin-top: 60px;
}

.testimonial-card {
background: var(--bg);
border-radius: 20px;
padding: 32px;
box-shadow: var(--shadow);
}

.testimonial-header {
display: flex;
align-items: center;
gap: 16px;
margin-bottom: 20px;
}

.testimonial-avatar {
width: 60px;
height: 60px;
background: linear-gradient(135deg, var(--primary), var(--secondary));
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
font-size: 24px;
color: white;
font-weight: 700;
}

.testimonial-info h4 {
font-size: 18px;
font-weight: 700;
color: var(--primary);
}

.testimonial-info span {
font-size: 14px;
color: var(--text-light);
}

.stars {
color: var(--accent);
font-size: 20px;
margin-bottom: 16px;
}

.testimonial-text {
font-size: 16px;
color: var(--text);
line-height: 1.7;
font-style: italic;
}

/* Location Section */
.location {
padding: 80px 20px;
background: var(--bg);
}

.location-content {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 60px;
align-items: center;
}

.location-info h2 {
font-size: 40px;
font-weight: 800;
color: var(--primary);
margin-bottom: 24px;
}

.location-details {
display: flex;
flex-direction: column;
gap: 20px;
margin-bottom: 32px;
}

.location-item {
display: flex;
align-items: start;
gap: 16px;
}

.location-icon {
width: 48px;
height: 48px;
background: var(--white);
border-radius: 12px;
display: flex;
align-items: center;
justify-content: center;
font-size: 24px;
flex-shrink: 0;
box-shadow: var(--shadow);
}

.location-item div strong {
display: block;
font-size: 16px;
color: var(--primary);
margin-bottom: 4px;
}

.location-item div span {
font-size: 15px;
color: var(--text-light);
}

.location-map {
background: linear-gradient(135deg, #e0e0e0, #f0f0f0);
border-radius: 24px;
height: 400px;
display: flex;
align-items: center;
justify-content: center;
font-size: 80px;
position: relative;
overflow: hidden;
}

.map-pin {
position: absolute;
background: var(--urgent);
color: white;
padding: 12px 20px;
border-radius: 12px;
font-weight: 700;
font-size: 14px;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
box-shadow: 0 4px 20px rgba(255,87,34,0.4);
}

/* CTA Section */
.cta-section {
padding: 100px 20px;
background: linear-gradient(135deg, var(--whatsapp-dark) 0%, var(--whatsapp) 100%);
color: var(--white);
text-align: center;
}

.cta-section h2 {
font-size: 48px;
font-weight: 800;
margin-bottom: 24px;
}

.cta-section p {
font-size: 20px;
opacity: 0.95;
max-width: 600px;
margin: 0 auto 40px;
}

.btn-cta-mega {
background: var(--white);
color: var(--whatsapp-dark);
padding: 24px 48px;
border-radius: 16px;
text-decoration: none;
font-size: 24px;
font-weight: 800;
display: inline-flex;
align-items: center;
gap: 16px;
transition: all 0.3s;
box-shadow: 0 12px 40px rgba(0,0,0,0.2);
animation: pulse-white 2s infinite;
}

@keyframes pulse-white {
0%, 100% { transform: scale(1); }
50% { transform: scale(1.05); }
}

.btn-cta-mega:hover {
transform: translateY(-4px);
box-shadow: 0 16px 50px rgba(0,0,0,0.3);
}

/* Footer */
.footer {
background: var(--primary-dark);
color: var(--white);
padding: 60px 20px 30px;
}

.footer-content {
max-width: 1200px;
margin: 0 auto;
display: grid;
grid-template-columns: 2fr 1fr 1fr 1fr;
gap: 40px;
margin-bottom: 40px;
}

.footer-brand h3 {
font-size: 24px;
font-weight: 800;
margin-bottom: 16px;
}

.footer-brand p {
font-size: 15px;
opacity: 0.8;
line-height: 1.7;
margin-bottom: 20px;
}

.footer-whatsapp {
display: inline-flex;
align-items: center;
gap: 8px;
background: var(--whatsapp);
color: var(--white);
padding: 12px 24px;
border-radius: 50px;
text-decoration: none;
font-weight: 700;
}

.footer-column h4 {
font-size: 16px;
font-weight: 700;
margin-bottom: 20px;
color: var(--accent);
}

.footer-column ul {
list-style: none;
}

.footer-column li {
margin-bottom: 12px;
}

.footer-column a {
color: rgba(255,255,255,0.8);
text-decoration: none;
font-size: 15px;
transition: color 0.3s;
}

.footer-column a:hover {
color: var(--white);
}

.footer-bottom {
border-top: 1px solid rgba(255,255,255,0.1);
padding-top: 30px;
text-align: center;
font-size: 14px;
opacity: 0.6;
}

/* Floating WhatsApp */
.whatsapp-float {
position: fixed;
bottom: 30px;
right: 30px;
background: var(--whatsapp);
color: var(--white);
width: 70px;
height: 70px;
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
font-size: 36px;
box-shadow: 0 8px 30px rgba(37,211,102,0.5);
cursor: pointer;
z-index: 9999;
animation: pulse-float 2s infinite;
text-decoration: none;
}

@keyframes pulse-float {
0%, 100% { transform: scale(1); box-shadow: 0 8px 30px rgba(37,211,102,0.5); }
50% { transform: scale(1.1); box-shadow: 0 12px 40px rgba(37,211,102,0.7); }
}

.whatsapp-tooltip {
position: absolute;
right: 80px;
background: var(--white);
color: var(--text);
padding: 12px 20px;
border-radius: 12px;
font-size: 14px;
font-weight: 600;
white-space: nowrap;
opacity: 0;
transform: translateX(10px);
transition: all 0.3s;
pointer-events: none;
box-shadow: var(--shadow);
}

.whatsapp-float:hover .whatsapp-tooltip {
opacity: 1;
transform: translateX(0);
}

/* Responsive */
@media (max-width: 1024px) {
.hero-text h1 {
font-size: 40px;
}

.options-grid {
grid-template-columns: 1fr;
}

.services-grid {
grid-template-columns: repeat(2, 1fr);
}

.process-steps {
grid-template-columns: 1fr;
}

.process-step::after {
display: none;
}

.testimonials-grid {
grid-template-columns: 1fr;
}

.location-content {
grid-template-columns: 1fr;
}

.footer-content {
grid-template-columns: 1fr 1fr;
}
}

@media (max-width: 768px) {
.header-contact {
display: none;
}

.menu-toggle {
display: block;
}

.hero {
padding: 120px 20px 60px;
}

.hero-text h1 {
font-size: 32px;
}

.survey-container {
padding: 24px;
}

.services-grid {
grid-template-columns: 1fr;
}

.footer-content {
grid-template-columns: 1fr;
text-align: center;
}

.whatsapp-float {
width: 60px;
height: 60px;
font-size: 30px;
bottom: 20px;
right: 20px;
}

.whatsapp-tooltip {
display: none;
}
}
</style>
</head>
<body>

<!-- Header -->
<header class="header">
<div class="header-content">
<div class="logo">
<div class="logo-icon">💰</div>
<span>Credimercuri</span>
</div>
<div class="header-contact">
<a href="https://wa.me/543544313118?text=Hola%20Credimercuri,%20vi%20su%20web%20y%20quiero%20información%20sobre%20préstamos" class="header-whatsapp" target="_blank">
<span>💬</span>
<span>WhatsApp</span>
</a>
</div>
<div class="menu-toggle">☰</div>
</div>
</header>

<!-- Hero Section -->
<section class="hero">
<div class="hero-content">
<div class="hero-text">
<h1>Préstamos en <span>24 horas</span> en Villa Dolores</h1>
<p class="hero-subtitle">Jubilados, pensionados, pensiones no contributivas y empleados. Sin garante, sin trámites engorrosos, con la confianza de un vecino.</p>

<div class="hero-features">
<div class="hero-feature">
<div class="hero-feature-icon">⚡</div>
<span>Aprobación en 24hs</span>
</div>
<div class="hero-feature">
<div class="hero-feature-icon">📍</div>
<span>Hipólito Yrigoyen 655</span>
</div>
<div class="hero-feature">
<div class="hero-feature-icon">✓</div>
<span>Sin garante</span>
</div>
</div>
</div>
</div>
</section>

<!-- SURVEY SECTION - COMPLETAMENTE NUEVA -->
<section class="survey-section" id="encuesta">
<div class="survey-container">
<div class="survey-header">
<h2>📋 Verificá tu préstamo en 1 minuto</h2>
<p>Respondé 4 preguntas y te diremos instantáneamente si calificás. Después te contactás por WhatsApp con los datos listos.</p>
</div>

<div class="survey-progress">
<div class="progress-dot active" id="dot-1"></div>
<div class="progress-dot" id="dot-2"></div>
<div class="progress-dot" id="dot-3"></div>
<div class="progress-dot" id="dot-4"></div>
</div>

<!-- STEP 1: Perfil -->
<div class="survey-step active" id="step-1">
<h3 class="question-title">¿Cuál es tu situación actual?</h3>
<p class="question-subtitle">Seleccioná la opción que mejor te describa</p>

<div class="options-grid">
<div class="option-card" onclick="selectOption(this, 'perfil', 'jubilado')">
<div class="option-icon">👴</div>
<div class="option-label">Jubilado/a</div>
<div class="option-hint">Anses o provincia</div>
</div>
<div class="option-card" onclick="selectOption(this, 'perfil', 'pensionado')">
<div class="option-icon">👵</div>
<div class="option-label">Pensionado/a</div>
<div class="option-hint">Viudez o invalidez</div>
</div>
<div class="option-card" onclick="selectOption(this, 'perfil', 'nocontributiva')">
<div class="option-icon">📝</div>
<div class="option-label">Pensión No Contributiva</div>
<div class="option-hint">Madres, veteranos, discapacidad</div>
</div>
<div class="option-card" onclick="selectOption(this, 'perfil', 'empleado')">
<div class="option-icon">💼</div>
<div class="option-label">Empleado/a</div>
<div class="option-hint">Relación de dependencia</div>
</div>
</div>

<div class="survey-buttons">
<button class="btn-survey btn-primary" onclick="nextStep(1)" disabled id="btn-step-1">
Continuar →
</button>
</div>
</div>

<!-- STEP 2: Banco -->
<div class="survey-step" id="step-2">
<h3 class="question-title">¿Dónde estás cobrando actualmente?</h3>
<p class="question-subtitle">Seleccioná el banco o entidad donde te depositan</p>

<div class="options-grid">
<div class="option-card" onclick="selectOption(this, 'banco', 'Anses')">
<div class="option-icon">🏛️</div>
<div class="option-label">Anses</div>
<div class="option-hint">Jubilaciones nacionales</div>
</div>
<div class="option-card" onclick="selectOption(this, 'banco', 'Banco Nación')">
<div class="option-icon">🏦</div>
<div class="option-label">Banco Nación</div>
<div class="option-hint">Provincia de Córdoba</div>
</div>
<div class="option-card" onclick="selectOption(this, 'banco', 'Banco Provincia')">
<div class="option-icon">🏛️</div>
<div class="option-label">Banco Provincia</div>
<div class="option-hint">Córdoba</div>
</div>
<div class="option-card" onclick="selectOption(this, 'banco', 'Banco Macro')">
<div class="option-icon">🏦</div>
<div class="option-label">Banco Macro</div>
<div class="option-hint">Otro banco privado</div>
</div>
<div class="option-card" onclick="selectOption(this, 'banco', 'Caja de Jubilaciones')">
<div class="option-icon">📮</div>
<div class="option-label">Caja de Jubilaciones</div>
<div class="option-hint">Provincial</div>
</div>
<div class="option-card" onclick="selectOption(this, 'banco', 'Otro')">
<div class="option-icon">💳</div>
<div class="option-label">Otro / No estoy seguro</div>
<div class="option-hint">Te ayudamos a verificar</div>
</div>
</div>

<div class="survey-buttons">
<button class="btn-survey btn-secondary" onclick="prevStep(2)">← Volver</button>
<button class="btn-survey btn-primary" onclick="nextStep(2)" disabled id="btn-step-2">
Continuar →
</button>
</div>
</div>

<!-- STEP 3: Monto del recibo -->
<div class="survey-step" id="step-3">
<h3 class="question-title">¿Cuál es el monto de tu recibo?</h3>
<p class="question-subtitle">Ingresá el monto bruto que figura en tu último recibo de sueldo, jubilación o pensión</p>

<div class="input-group" style="max-width: 400px; margin: 0 auto;">
<label>Monto del recibo (en pesos argentinos)</label>
<input type="number" id="monto-recibo" placeholder="Ej: 185000" oninput="updateMontoRecibo(this.value)">
<p class="input-hint">Sin puntos ni comas. Ejemplo: si cobrás $185.230, escribí 185230</p>
</div>

<div class="amount-display" id="monto-display" style="display: none;">
<h4>Monto ingresado:</h4>
<div class="amount" id="monto-formateado">$0</div>
</div>

<div class="survey-buttons">
<button class="btn-survey btn-secondary" onclick="prevStep(3)">← Volver</button>
<button class="btn-survey btn-primary" onclick="nextStep(3)" disabled id="btn-step-3">
Continuar →
</button>
</div>
</div>

<!-- STEP 4: Cuánto le queda en mano -->
<div class="survey-step" id="step-4">
<h3 class="question-title">¿Cuánto te queda en mano?</h3>
<p class="question-subtitle">Ingresá el monto neto que realmente recibís después de todos los descuentos</p>

<div class="input-group" style="max-width: 400px; margin: 0 auto;">
<label>Monto neto en mano (en pesos argentinos)</label>
<input type="number" id="monto-mano" placeholder="Ej: 145000" oninput="updateMontoMano(this.value)">
<p class="input-hint">Lo que realmente te queda para gastar después de descuentos</p>
</div>

<div class="amount-display" id="mano-display" style="display: none; background: linear-gradient(135deg, #e8f5e9, #c8e6c9);">
<h4>Disponible mensual:</h4>
<div class="amount" id="mano-formateado" style="color: #2e7d32;">$0</div>
</div>

<div style="background: #fff3e0; border-radius: 12px; padding: 16px; margin-top: 24px; text-align: center;">
<p style="font-size: 14px; color: #e65100; margin: 0;">
💡 <strong>Tip:</strong> Con este dato calculamos cuánto podés pagar cómodamente por mes
</p>
</div>

<div class="survey-buttons">
<button class="btn-survey btn-secondary" onclick="prevStep(4)">← Volver</button>
<button class="btn-survey btn-primary" onclick="finishSurvey()" disabled id="btn-step-4">
Ver resultado →
</button>
</div>
</div>

<!-- RESULT STEP -->
<div class="survey-step" id="step-result">
<div id="result-content">
<!-- Se llena dinámicamente con JavaScript -->
</div>
</div>

</div>
</section>

<!-- Services Section -->
<section class="services">
<div class="container">
<div class="section-header">
<h2>¿A quiénes ayudamos?</h2>
<p>Tenemos opciones pensadas para diferentes situaciones. Todos merecen una segunda oportunidad financiera.</p>
</div>

<div class="services-grid">
<div class="service-card">
<div class="service-icon">👴</div>
<h3>Jubilados</h3>
<p>Préstamos pensados para adultos mayores. Sin garante, cuotas que no superan el 30% de la jubilación.</p>
</div>

<div class="service-card">
<div class="service-icon">👵</div>
<h3>Pensionados</h3>
<p>Aprobación garantizada para quienes cobran pensión. Entendemos que cada peso cuenta.</p>
</div>

<div class="service-card">
<div class="service-icon">📝</div>
<h3>Pensiones No Contributivas</h3>
<p>Madres de 7 hijos, invalidez, veteranos: aprobamos donde otros dicen NO.</p>
</div>

<div class="service-card">
<div class="service-icon">💼</div>
<h3>Empleados</h3>
<p>Con o sin recibo de sueldo. Hasta 3 sueldos de préstamo. Aprobación express.</p>
</div>
</div>
</div>
</section>

<!-- Process Section -->
<section class="process">
<div class="container">
<div class="section-header">
<h2>Así de fácil es obtener tu préstamo</h2>
<p>Tres pasos simples, sin vueltas. Desde que entrás por la puerta hasta tener la plata en tu mano.</p>
</div>

<div class="process-steps">
<div class="process-step">
<div class="step-number">1</div>
<h3>Vení con tu documentación</h3>
<p>Solo necesitás DNI, último recibo de sueldo/jubilación y un servicio a tu nombre.</p>
</div>

<div class="process-step">
<div class="step-number">2</div>
<h3>Evaluamos en el momento</h3>
<p>Analizamos tu situación en el acto. Sin esperar días ni semanas.</p>
</div>

<div class="process-step">
<div class="step-number">3</div>
<h3>En 24hs tenés la plata</h3>
<p>Una vez aprobado, en 24 horas hábiles tenés el dinero.</p>
</div>
</div>
</div>
</section>

<!-- Testimonials -->
<section class="testimonials">
<div class="container">
<div class="section-header">
<h2>Lo que dicen nuestros clientes</h2>
<p>Historias reales de vecinos de Villa Dolores y la zona.</p>
</div>

<div class="testimonials-grid">
<div class="testimonial-card">
<div class="testimonial-header">
<div class="testimonial-avatar">MR</div>
<div class="testimonial-info">
<h4>María R.</h4>
<span>Jubilada • Villa Dolores</span>
</div>
</div>
<div class="stars">★★★★★</div>
<p class="testimonial-text">"Mi banco me dijo que no por mi edad. Vine a Credimercuri y en 2 días tenía la plata. Guille me trató con respeto."</p>
</div>

<div class="testimonial-card">
<div class="testimonial-header">
<div class="testimonial-avatar" style="background: linear-gradient(135deg, #9c27b0, #e91e63);">JL</div>
<div class="testimonial-info">
<h4>José L.</h4>
<span>Pensión No Contributiva</span>
</div>
</div>
<div class="stars">★★★★★</div>
<p class="testimonial-text">"Cobro pensión por discapacidad y en todos lados me rechazaban. Guille fue el único que me dio una oportunidad."</p>
</div>

<div class="testimonial-card">
<div class="testimonial-header">
<div class="testimonial-avatar" style="background: linear-gradient(135deg, #ff9800, #f44336);">CG</div>
<div class="testimonial-info">
<h4>Carlos G.</h4>
<span>Empleado • Valle de Traslasierra</span>
</div>
</div>
<div class="stars">★★★★★</div>
<p class="testimonial-text">"Se me rompió el auto y lo necesitaba para trabajar. Guille me aprobó el préstamo en el día. Gente de palabra."</p>
</div>
</div>
</div>
</section>

<!-- Location Section -->
<section class="location">
<div class="container">
<div class="location-content">
<div class="location-info">
<h2>Vení a conocernos</h2>
<p style="font-size: 18px; color: var(--text-light); margin-bottom: 32px;">
Local físico en el centro de Villa Dolores. Atendemos con la cara visible.
</p>

<div class="location-details">
<div class="location-item">
<div class="location-icon">📍</div>
<div>
<strong>Dirección</strong>
<span>Hipólito Yrigoyen 655, Villa Dolores, Córdoba</span>
</div>
</div>

<div class="location-item">
<div class="location-icon">🕐</div>
<div>
<strong>Horario</strong>
<span>Lunes a Viernes: 9:00 a 18:00 hs</span>
</div>
</div>

<div class="location-item">
<div class="location-icon">📱</div>
<div>
<strong>WhatsApp</strong>
<span>+54 9 3544 31-3118</span>
</div>
</div>
</div>
</div>

<div class="location-map">
🗺️
<div class="map-pin">📍 Estamos aquí</div>
</div>
</div>
</div>
</section>

<!-- CTA Section -->
<section class="cta-section">
<h2>¿Listo para solucionar tu situación?</h2>
<p>No esperes más. Escribime ahora por WhatsApp y en 5 minutos te digo cuánto puedo ayudarte.</p>
<a href="https://wa.me/543544313118?text=Hola%20Guille,%20completé%20la%20encuesta%20en%20la%20web%20y%20quiero%20consultar" class="btn-cta-mega" target="_blank">
<span>💬</span>
<span>Escribir por WhatsApp ahora</span>
</a>
</section>

<!-- Footer -->
<footer class="footer">
<div class="footer-content">
<div class="footer-brand">
<h3>💰 Credimercuri</h3>
<p>Préstamos personales con respaldo humano. Más de 10 años en Villa Dolores.</p>
<a href="https://wa.me/543544313118" class="footer-whatsapp" target="_blank">
<span>💬</span>
<span>+54 9 3544 31-3118</span>
</a>
</div>

<div class="footer-column">
<h4>Servicios</h4>
<ul>
<li><a href="#">Jubilados</a></li>
<li><a href="#">Pensionados</a></li>
<li><a href="#">Pensiones No Contributivas</a></li>
<li><a href="#">Empleados</a></li>
</ul>
</div>

<div class="footer-column">
<h4>Enlaces</h4>
<ul>
<li><a href="#encuesta">Verificar préstamo</a></li>
<li><a href="#">Cómo llegar</a></li>
<li><a href="#">Testimonios</a></li>
</ul>
</div>

<div class="footer-column">
<h4>Legal</h4>
<ul>
<li><a href="#">Términos y condiciones</a></li>
<li><a href="#">Privacidad</a></li>
</ul>
</div>
</div>

<div class="footer-bottom">
<p>© 2024 Credimercuri - Hipólito Yrigoyen 655, Villa Dolores, Córdoba</p>
</div>
</footer>

<!-- Floating WhatsApp -->
<a href="https://wa.me/543544313118?text=Hola%20Guille,%20vi%20la%20web%20y%20quiero%20consultar" class="whatsapp-float" target="_blank">
💬
<span class="whatsapp-tooltip">¡Escribime ahora!</span>
</a>

<script>
// Survey State
let surveyData = {
perfil: '',
banco: '',
montoRecibo: 0,
montoMano: 0
};

let currentStep = 1;

function selectOption(element, field, value) {
// Remove selected from siblings
const parent = element.parentElement;
const siblings = parent.querySelectorAll('.option-card');
siblings.forEach(sib => sib.classList.remove('selected'));

// Add selected to clicked
element.classList.add('selected');

// Save data
surveyData[field] = value;

// Enable next button
document.getElementById(`btn-step-${currentStep}`).disabled = false;
}

function updateMontoRecibo(value) {
surveyData.montoRecibo = parseFloat(value) || 0;

const display = document.getElementById('monto-display');
const formateado = document.getElementById('monto-formateado');

if (surveyData.montoRecibo > 0) {
display.style.display = 'block';
formateado.textContent = '$' + surveyData.montoRecibo.toLocaleString('es-AR');
document.getElementById('btn-step-3').disabled = false;
} else {
display.style.display = 'none';
document.getElementById('btn-step-3').disabled = true;
}
}

function updateMontoMano(value) {
surveyData.montoMano = parseFloat(value) || 0;

const display = document.getElementById('mano-display');
const formateado = document.getElementById('mano-formateado');

if (surveyData.montoMano > 0) {
display.style.display = 'block';
formateado.textContent = '$' + surveyData.montoMano.toLocaleString('es-AR');
document.getElementById('btn-step-4').disabled = false;
} else {
display.style.display = 'none';
document.getElementById('btn-step-4').disabled = true;
}
}

function nextStep(step) {
// Hide current step
document.getElementById(`step-${step}`).classList.remove('active');

// Update progress dots
document.getElementById(`dot-${step}`).classList.remove('active');
document.getElementById(`dot-${step}`).classList.add('completed');

// Show next step
currentStep = step + 1;
document.getElementById(`step-${currentStep}`).classList.add('active');
document.getElementById(`dot-${currentStep}`).classList.add('active');
}

function prevStep(step) {
// Hide current step
document.getElementById(`step-${step}`).classList.remove('active');

// Update progress dots
document.getElementById(`dot-${step}`).classList.remove('active');

// Show previous step
currentStep = step - 1;
document.getElementById(`step-${currentStep}`).classList.add('active');
document.getElementById(`dot-${currentStep}`).classList.remove('completed');
document.getElementById(`dot-${currentStep}`).classList.add('active');
}

function finishSurvey() {
// Hide step 4
document.getElementById('step-4').clas
...
