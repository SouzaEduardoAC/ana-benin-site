<script setup lang="ts">
import anaImage from '@/assets/aaacdad5-f3eb-41c0-a587-f0f49495c92c.jpeg'
</script>

<template>
  <section class="hero">
    <div class="hero-split">
      <div class="hero-image">
        <img :src="anaImage" alt="Dra. Ana Benin">
      </div>
      <div class="hero-content-side">
        <div class="hero-content">
          <div class="badge-hero">CRM-SC 20559 | RQE 15294 / 20078</div>
          <h1>Neurologia e Clínica Médica com visão integral da sua saúde</h1>
          <p>Diagnóstico preciso e tratamento humanizado baseado em evidências. 
            <strong>Atendimento especializado em Blumenau.</strong></p>
          
          <div class="cta-group">
            <a href="https://wa.me/5547996987678" class="btn btn-primary" target="_blank"><i class="fa-brands fa-whatsapp"></i> Agendar Minha Consulta</a>
            <a href="#servicos" class="btn btn-outline">Conhecer Serviços <i class="fa-solid fa-arrow-right"></i></a>
          </div>

          <div class="meso-clinic-info">
            <i class="fa-solid fa-location-dot"></i> Atendimento na MesoClinic - Ambiente acolhedor e moderno
          </div>
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
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: var(--bg-beige);
  overflow: hidden;
}

.hero-split {
  display: flex;
  flex: 1;
  width: 100%;
}

.hero-image {
  flex: 0.8;
  position: relative;
  display: flex;
  align-items: flex-end;
  justify-content: center;
  background-color: #e5e7eb;
}

.hero-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center 15%;
}

.hero-content-side {
  flex: 1.2;
  background-color: var(--bg-dark-green-graysh);
  display: flex;
  align-items: center;
  padding: 4.5% 7%;
  color: white;
  z-index: 2;
}

.hero-content {
  max-width: 550px;
}

.badge-hero {
  display: inline-block;
  background: rgba(255,255,255,0.1);
  padding: 5px 14px;
  border-radius: 20px;
  font-size: 0.78rem;
  margin-bottom: 1.75rem;
  border: 1px solid rgba(255,255,255,0.2);
  letter-spacing: 0.5px;
}

.hero h1 {
  font-size: 3.0rem;
  line-height: 1.12;
  margin-bottom: 1.4rem;
  font-weight: 600;
}

.hero p {
  font-size: 1.1rem;
  color: #e5e7eb;
  margin-bottom: 2.2rem;
  line-height: 1.55;
}

.cta-group { 
  display: flex; 
  gap: 1.2rem;
  margin-bottom: 1.75rem;
}

.meso-clinic-info {
  font-size: 0.88rem;
  color: #9ca3af;
  display: flex;
  align-items: center;
  gap: 10px;
}

.meso-clinic-info i {
  color: var(--accent-brown);
}

/* Wave */
.wave-bottom {
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  line-height: 0;
  z-index: 3;
}
.wave-bottom svg {
  display: block;
  width: 100%;
  height: 70px;
}
.wave-bottom .shape-fill { fill: var(--bg-beige); }

@media (max-width: 1024px) {
  .hero h1 { font-size: 2.8rem; }
}

@media (max-width: 850px) {
  .hero {
    height: auto;
  }
  .hero-split {
    flex-direction: column;
  }
  .hero-image {
    height: 40vh;
    flex: none;
  }
  .hero-content-side {
    padding: 6.5rem 1.5rem 4.5rem;
  }
  .hero h1 { font-size: 2.2rem; }
  .wave-bottom {
    display: none;
  }
  .cta-group {
    flex-direction: column;
    width: 100%;
  }
  .btn {
    width: 100%;
  }
}
</style>