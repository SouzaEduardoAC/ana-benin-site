<script setup lang="ts"></script>

<template>
  <section class="services-section" id="servicos">
    <div class="container">
      <div class="section-title">
        <h2>Compromisso em promover neuroprevenção, preservar e recuperar autonomia e qualidade de vida</h2>
        <p>Atuamos na investigação, diagnóstico e tratamento de condições que afetam o sistema nervoso central e periférico.</p>
      </div>

      <div class="services-grid">
        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Dores de cabeça e Enxaqueca</h3>
          <p>Bloqueios anestésicos em cefaleias</p>
          <p>Toxina Botulínica</p>
          <p>Anticorpos monoclonais (vacinas)</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Neuromodulação não-invasiva</h3>
          <p>Estimulação Magnética transcraniana - EMT (TMS)</p>
          <p>Estimulação trascraniana por corrente contínua (ETCC/TDCS)</p>
        </article>
        
        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Reabilitação neurológica</h3>
          <p>Fibromialgia e Dor Crônica</p>
          <p>AVC</p>
          <p>Distúrbios de Movimento (Ataxias, Parkinson)</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Longevidade e Saúde do Cérebro</h3>
          <p>Plano de ação em medicina do estilo de vida e neuroprevenção de doenças neurodegenerativas e perda de autonomia</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Consulta em Neurologia e Clínica Médica</h3>
          <p>Acompanhamento em Consultório, Domiciliar e Hospitalar</p>
        </article>

      </div>
    </div>
  </section>
</template>

<style scoped>
.services-section {
  background-color: var(--bg-dark-green);
  padding: 5rem 0;
  color: var(--text-light);
  text-align: center;
  min-height: 95vh;
  display: flex;
  align-items: center;
}

.section-title h2 {
  font-size: 2.2rem;
  margin-bottom: 1rem;
  line-height: 1.2;
}

.section-title p {
  color: #bbb;
  max-width: 700px;
  margin: 0 auto 3rem;
  font-size: 1.1rem;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  text-align: left;
}

@media (max-width: 850px) {
  .services-section {
    padding: 6rem 0;
    height: auto;
  }
  .section-title h2 {
    font-size: 1.8rem;
  }
}

.service-card {
  background: var(--bg-beige);
  border: 1px solid rgba(0,0,0,0.05);
  padding: 1.5rem;
  border-radius: 12px;
  transition: 0.3s;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  display: flex;
  flex-direction: column;
  height: 100%;
}
.service-card:hover { transform: translateY(-5px); box-shadow: 0 8px 25px rgba(0,0,0,0.15); }

.service-icon {
  background: var(--primary-green);
  width: 40px; height: 40px;
  display: flex; align-items: center; justify-content: center;
  border-radius: 8px;
  margin-bottom: 1rem;
  font-size: 1.1rem;
  color: #fff;
}

.service-card h3 { font-size: 1.15rem; margin-bottom: 0.75rem; color: var(--bg-dark-green); font-weight: 600; line-height: 1.3; }
.service-card p { font-size: 0.9rem; color: var(--text-gray); margin-bottom: 0.5rem; line-height: 1.4; }
.service-card i.fa-check { color: var(--primary-green); font-size: 0.8rem; margin-right: 5px; display: inline-block; }
.service-card p:last-child { margin-bottom: 0; }

.service-checks i { color: #DACBA9; margin-right: 8px; font-size: 0.8rem; }
.service-checks div { margin-bottom: 5px; font-size: 0.85rem; color: #ddd; }

.when-to-seek {
  background: #503b28;
  border-radius: 12px;
  padding: 1.5rem;
  text-align: center;
  margin-top: 1.5rem;
}

.seek-title {
  color: white; 
  margin-bottom: 0.5rem;
  font-size: 1.2rem;
}

.when-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.8rem;
  text-align: left;
  margin: 1rem 0;
}
.when-item { font-size: 0.8rem; color: #f0f0f0; }
.when-item::before { content: '●'; color: #DACBA9; margin-right: 8px; }

.btn-white {
  background: white;
  color: #333;
}
</style>
