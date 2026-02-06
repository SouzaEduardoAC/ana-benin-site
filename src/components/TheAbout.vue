<script setup lang="ts">
import anaImage from '@/assets/foto_ana_benin.png'
</script>

<template>
  <section class="about-section" id="sobre">
    <div class="container">
      <div class="about-grid">
        <!-- <div class="about-img">
          <img :src="anaImage" alt="Mãos Médicas">
        </div> -->
        <div class="about-text">
          <h3>Compromisso com a sua história clínica</h3>
          <h1>Dra. Ana Benin</h1>
          <div class="badges-crm">
            <span class="crm-tag legal-id">CRM-SC 20559</span>
            <span class="crm-tag legal-id">RQE 15294</span>
            <span class="crm-tag legal-id">RQE 20078</span>
          </div>

          <p>
            A medicina vai muito além de tratar sintomas ou de tecnologias avançadas; trata-se de compreender a pessoa.
            Sou a <strong>Dra. Ana Caroline Benin</strong>, médica especialista em Neurologia e Medicina Interna.
          </p>
          <p>
            Minha prática clínica une o rigor técnico da especialidade com uma escuta ativa e ética. 
            Acredito que um diagnóstico correto é o primeiro passo para recuperar a liberdade de viver bem e fazer boas escolhas.
          </p>

          <div class="mini-cards">
            <div class="mini-card">
              <i class="fa-solid fa-brain"></i>
              <div>
                <h5>Residência em Clínica Médica</h5>
                <span>Hospital Santa Isabel, Blumenau</span>
              </div>
            </div>
            <div class="mini-card">
              <i class="fa-solid fa-head-side-virus"></i>
              <div>
                <h5>Residência em Neurologia</h5>
                <span>Hospital Santa Isabel, Blumenau</span>
              </div>
            </div>
            <div class="mini-card">
              <i class="fa-solid fa-hospital-user"></i>
              <div>
                <h5>Pós Graduação em Neurointensivismo</h5>
                <span>Hospital Israelita Albert Einstein</span>
              </div>
            </div>
            <div class="mini-card">
              <i class="fa-solid fa-stethoscope"></i>
              <div>
                <h5>Aprimoramento em Neuromodulação e Neurofisiologia</h5>
                <span>Rede SARAH Brasília</span>
              </div>
            </div>
            <div class="mini-card">
              <i class="fa-solid fa-stethoscope"></i>
              <div>
                <h5>Aprimoramento em Neuromodulação</h5>
                <span>UNIFESP</span>
              </div>
            </div>
            <div class="mini-card">
              <i class="fa-solid fa-stethoscope"></i>
              <div>
                <h5>Membro das Sociedades</h5>
                <span>Sociedade Brasileira de Cefaleia (SBCe)</span>
                <br />
                <span>Sociedade Internacional de Neuromodulação (INS)</span>
                <br />
                <span>Academia Brasileira de Neurologia (ABN)</span>
              </div>
            </div>
          </div>

          <a href="http://lattes.cnpq.br/7371424791523298" target="_blank" rel="noopener noreferrer" class="btn btn-primary">Ver Currículo Lattes<i class="fa-solid fa-arrow-right"></i></a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about-section {
  background-color: var(--bg-beige);
  padding: 4rem 0;
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.about-img {
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.about-text h4 {
  color: var(--accent-brown);
  text-transform: uppercase;
  letter-spacing: 1px;
  font-size: 0.85rem;
  margin-bottom: 0.5rem;
}

.about-text h2 {
  font-size: 2.5rem;
  color: #2c2c2c;
  margin-bottom: 1rem;
}

.badges-crm {
  display: flex;
  gap: 10px;
  margin-bottom: 1.5rem;
}
.crm-tag {
  background: #3A3A3A;
  color: white;
  padding: 4px 12px;
  border-radius: 20px;
  font-size: 0.75rem;
}

.about-text p {
  color: var(--text-gray);
  margin-bottom: 1rem;
  font-size: 0.95rem;
}

.mini-cards {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
  margin-top: 2rem;
  margin-bottom: 2rem;
}

.mini-card {
  background: white;
  padding: 1rem;
  border-radius: 8px;
  display: flex;
  align-items: center;
  gap: 10px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}
.mini-card i { font-size: 1.5rem; color: var(--primary-green); }
.mini-card div h5 { font-size: 0.9rem; margin-bottom: 2px; }
.mini-card div span { font-size: 0.75rem; color: #777; }

.lattes-link {
  margin-left: 15px;
  font-size: 0.9rem;
  color: #666;
  text-decoration: underline;
}

@media (max-width: 900px) {
  .about-grid { grid-template-columns: 1fr; }
}
</style>
