<script setup lang="ts"></script>

<template>
  <section class="services-section" id="servicos">
    <div class="container">
      <div class="section-title">
        <h3>Áreas de Atuação</h3>
        <h2>Cuidado neurológico focado na sua qualidade de vida</h2>
        <p>Atuamos na investigação, diagnóstico e acompanhamento de condições que afetam o sistema nervoso central e periférico.</p>
      </div>

      <div class="services-grid">
        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Cefaleias e Enxaquecas</h3>
          <p>Manejo da dor para você retomar sua rotina.</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Transtornos de Memória</h3>
          <p>Investigação de Alzheimer e outras demências com acolhimento familiar.</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Doenças Cerebrovasculares (AVC)</h3>
          <p>Prevenção e acompanhamento pós-evento.</p>
        </article>

        <article class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Transtornos do Movimento</h3>
          <p>Parkinson, tremores e ataxias.</p>
        </article>





<!-- 
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-brain"></i></div>
          <h3>Neurologia Geral</h3>
          <p>Avaliação completa de alterações neurológicas, incluindo memória, tontura, formigamento e tremores.</p>
          <div class="service-checks">
            <div><i class="fa-solid fa-check"></i> Avaliação diagnóstica precisa</div>
            <div><i class="fa-solid fa-check"></i> Tratamentos atualizados</div>
          </div>
        </div>
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-shield-halved"></i></div>
          <h3>Neuroprevenção</h3>
          <p>Avaliação preventiva e estratégias para manter a saúde cerebral, reduzindo riscos de doenças.</p>
        </div>
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-head-side-cough"></i></div>
          <h3>Tratamento de Cefaleias</h3>
          <p>Especialização em enxaquecas, dores de cabeça tensionais e outros tipos com abordagens modernas.</p>
          <div class="service-checks">
            <div><i class="fa-solid fa-check"></i> Diagnóstico específico</div>
            <div><i class="fa-solid fa-check"></i> Plano terapêutico personalizado</div>
          </div>
        </div>
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-bolt"></i></div>
          <h3>Neuromodulação</h3>
          <p>Técnicas avançadas de estimulação cerebral para tratamento de dores crônicas e enxaquecas.</p>
          <div class="service-checks">
            <div><i class="fa-solid fa-check"></i> Formação SARAH e UNIFESP</div>
            <div><i class="fa-solid fa-check"></i> Tecnologia de ponta</div>
          </div>
        </div>
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-hand-holding-heart"></i></div>
          <h3>Neurorreabilitação</h3>
          <p>Recuperação funcional após AVC, traumatismos e outras lesões neurológicas com plano individualizado.</p>
        </div>
        <div class="service-card">
          <div class="service-icon"><i class="fa-solid fa-bed-pulse"></i></div>
          <h3>Neurointensivismo</h3>
          <p>Acompanhamento especializado pós-internação e cuidados intensivos neurológicos com formação Einstein.</p>
        </div> -->
        
      </div>

      <!-- <div class="when-to-seek">
        <h3 class="seek-title">Quando Procurar um Neurologista?</h3>
        <div class="when-grid">
          <div class="when-item">Dores de cabeça frequentes</div>
          <div class="when-item">Tonturas e vertigens</div>
          <div class="when-item">Alterações de memória</div>
          <div class="when-item">Formigamentos inexplicados</div>
          <div class="when-item">Tremores involuntários</div>
          <div class="when-item">Dificuldade de concentração</div>
        </div>
        <button class="btn btn-white">Ver Todos os Serviços <i class="fa-solid fa-arrow-right"></i></button>
      </div> -->
    </div>
  </section>
</template>

<style scoped>
.services-section {
  background-color: var(--bg-dark-green);
  padding: 4rem 0;
  color: var(--text-light);
  text-align: center;
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.section-title h4 {
  color: #aaa;
  text-transform: uppercase;
  font-size: 0.8rem;
  letter-spacing: 1px;
  margin-bottom: 10px;
}

.section-title h2 {
  font-size: 2.2rem;
  margin-bottom: 1rem;
}

.section-title p {
  color: #bbb;
  max-width: 600px;
  margin: 0 auto 4rem;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  text-align: left;
  margin-bottom: 4rem;
}

.service-card {
  background: var(--bg-beige);
  border: 1px solid rgba(0,0,0,0.05);
  padding: 2.5rem 2rem;
  border-radius: 12px;
  transition: 0.3s;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}
.service-card:hover { transform: translateY(-5px); box-shadow: 0 8px 25px rgba(0,0,0,0.15); }

.service-icon {
  background: var(--primary-green);
  width: 50px; height: 50px;
  display: flex; align-items: center; justify-content: center;
  border-radius: 8px;
  margin-bottom: 1.5rem;
  font-size: 1.2rem;
  color: #fff;
}

.service-card h3 { font-size: 1.25rem; margin-bottom: 1rem; color: var(--bg-dark-green); font-weight: 600; }
.service-card p { font-size: 0.95rem; color: var(--text-gray); margin-bottom: 0; }

.service-checks i { color: #DACBA9; margin-right: 8px; font-size: 0.8rem; }
.service-checks div { margin-bottom: 5px; font-size: 0.85rem; color: #ddd; }

.when-to-seek {
  background: #503b28;
  border-radius: 12px;
  padding: 3rem;
  text-align: center;
}

.seek-title {
  color: white; 
  margin-bottom: 1rem;
}

.when-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
  text-align: left;
  margin: 2rem 0;
}
.when-item { font-size: 0.9rem; color: #f0f0f0; }
.when-item::before { content: '●'; color: #DACBA9; margin-right: 8px; }

.btn-white {
  background: white;
  color: #333;
}
</style>
