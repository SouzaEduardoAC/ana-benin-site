<script setup lang="ts">
import backgroundImage from '@/assets/the_hero_background.png'
</script>

<template>
  <section class="hero" :style="{ '--bg-image': `url(${backgroundImage})` }">
    <div class="container">
      <div class="hero-content">
        <div class="badge-hero">CRM-SC 20559 | RQE 15294 / 20078</div>
        <h1>Neurologia e Medicina Interna com visão integral da sua saúde</h1>
        <p>Diagnóstico preciso e tratamento humanizado baseado em evidências. 
          <strong>Atendimento especializado em Blumenau.</strong></p>
        
        <div class="cta-group">
          <a href="https://wa.me/5547996987678" class="btn btn-primary" target="_blank"><i class="fa-brands fa-whatsapp"></i> Agendar Minha Consulta</a>
          <!-- <a href="#servicos" class="btn btn-outline">Conhecer Serviços <i class="fa-solid fa-arrow-right"></i></a> -->
        </div>

        <div class="meso-clinic-info">
          <i class="fa-solid fa-location-dot"></i> Atendimento na MesoClinic - Ambiente acolhedor e moderno
        </div>
      </div>
    </div>
    <div class="wave-bottom">
      <svg viewBox="0 0 1200 120" preserveAspectRatio="none">
        <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
      </svg>
    </div>
  </section>
</template>

<style scoped>
.hero {
  position: relative;
  background: var(--bg-image) center/cover;
  min-height: 100vh;
  display: flex;
  align-items: center;
  color: white;
}

.hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(73, 73, 72, 0.85); /* Overlay escuro */
}

.hero-content {
  position: relative;
  z-index: 2;
  max-width: 650px;
}

.badge-hero {
  display: inline-block;
  background: rgba(255,255,255,0.15);
  padding: 5px 15px;
  border-radius: 20px;
  font-size: 0.8rem;
  margin-bottom: 1.5rem;
  border: 1px solid rgba(255,255,255,0.2);
}

.hero h1 {
  font-size: 3.5rem;
  line-height: 1.2;
  margin-bottom: 1.5rem;
}
.hero h1 span { color: #DACBA9; }

.hero p {
  font-size: 1.1rem;
  color: #d1d5db;
  margin-bottom: 2rem;
}

.hero-icons {
  display: flex;
  gap: 20px;
  margin-bottom: 2.5rem;
  font-size: 0.9rem;
  color: #ccc;
}
.hero-icons i { color: #DACBA9; margin-right: 5px; }

.cta-group { display: flex; gap: 1rem; }

.meso-clinic-info {
  margin-top: 20px;
  font-size: 0.85rem;
  color: #aaa;
  display: flex;
  align-items: center;
  gap: 8px;
}

/* Divisor de Onda (Wave) */
.wave-bottom {
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}
.wave-bottom svg {
  display: block;
  width: calc(100% + 1.3px);
  height: 80px;
}
.wave-bottom .shape-fill { fill: var(--bg-beige); }

@media (max-width: 900px) {
  .hero h1 { font-size: 2.5rem; }
}
</style>
