<script setup lang="ts"></script>

<template>
  <section class="media-section">
    <div class="container">
      <div class="media-header">
        <small>NA MÍDIA</small>
        <h2>Neuromodulação em <span>Destaque</span></h2>
        <p>Conheça mais sobre as tecnologias avançadas que utilizamos.</p>
      </div>

      <div class="news-card">
        <div class="news-img">
          <span class="g1-badge"><i class="fa-regular fa-newspaper"></i> G1 Santa Catarina</span>
        </div>
        <div class="news-content">
          <div class="news-meta">
            <span><i class="fa-regular fa-calendar"></i> 22 de Julho, 2025</span>
            <span><i class="fa-regular fa-clock"></i> 5 min de leitura</span>
          </div>
          <h3>Neuromodulação: Tecnologia de Ponta Ajuda o Cérebro a Reaprender</h3>
          <p>Descubra como a neuromodulação está revolucionando o tratamento de condições neurológicas, utilizando tecnologia avançada para estimular o cérebro e promover a recuperação funcional.</p>
          
          <div class="news-checks">
            <div><i class="fa-solid fa-circle-check"></i> Tratamentos inovadores para dores crônicas e depressões resistentes </div>
            <div><i class="fa-solid fa-circle-check"></i> Recuperação neurológica com tecnologia de ponta </div>
            <div><i class="fa-solid fa-circle-check"></i> Resultados comprovados cientificamente</div>
          </div>

          <a href="https://g1.globo.com/sc/santa-catarina/especial-publicitario/mesoclinic/noticia/2025/07/22/neuromodulacao-tecnologia-de-ponta-ajuda-o-cerebro-a-reaprender.ghtml" target="_blank" rel="noopener noreferrer" class="btn btn-primary">Ler Matéria Completa <i class="fa-solid fa-arrow-up-right-from-square"></i></a>
          <p class="news-caption">Publicação especial da MesoClinic no G1 Santa Catarina</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.media-section {
  background-color: var(--bg-beige);
  padding: 4rem 0;
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.media-header { text-align: center; margin-bottom: 3rem; }
.media-header h2 { font-size: 2.2rem; color: #1a1a1a; margin-bottom: 0.5rem; }
.media-header h2 span { display: block; font-size: 2rem; font-weight: 700; color: #2F3E33; }

.news-card {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  display: grid;
  grid-template-columns: 0.8fr 1.2fr;
  box-shadow: 0 5px 20px rgba(0,0,0,0.05);
  margin-bottom: 2rem;
}

.news-img {
  background: url('https://s2-g1.glbimg.com/6piyGBOEarzvtSbMWMYzN7ifHjQ=/0x0:853x1280/984x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_59edd422c0c84a879bd37670ae4f538a/internal_photos/bs/2025/U/z/zIXgNpRQCCgAmUB16PTQ/whatsapp-image-2025-07-24-at-14.35.17.jpeg') center/cover;
  position: relative;
  min-height: 300px; /* Ensure height if empty */
}
.g1-badge {
  position: absolute;
  top: 20px; left: 20px;
  background: #2E5E38;
  color: white;
  padding: 5px 12px;
  font-size: 0.7rem;
  border-radius: 4px;
  font-weight: bold;
}

.news-content { padding: 3rem; }
.news-meta { color: #888; font-size: 0.8rem; margin-bottom: 1rem; display: flex; align-items: center; gap: 10px; }
.news-content h3 { font-size: 1.8rem; margin-bottom: 1rem; color: #222; }
.news-content p { color: #666; margin-bottom: 1.5rem; line-height: 1.7; }

.news-checks { margin-bottom: 2rem; }
.news-checks div { display: flex; gap: 10px; margin-bottom: 8px; color: #555; font-size: 0.9rem; }
.news-checks i { color: var(--primary-green); margin-top: 4px; }

.news-caption {
  margin-top: 20px; 
  font-size: 0.75rem; 
  color: #aaa; 
  font-style: italic;
}

.stats-row {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
}
.stat-card {
  padding: 2rem;
  border-radius: 8px;
  text-align: center;
  color: white;
}
.stat-card i { font-size: 1.5rem; margin-bottom: 1rem; background: rgba(255,255,255,0.2); width: 50px; height: 50px; display: inline-flex; align-items: center; justify-content: center; border-radius: 50%; }
.stat-card h5 { font-size: 1rem; margin-bottom: 0.5rem; }
.stat-card p { font-size: 0.8rem; opacity: 0.8; }

.bg-olive { background-color: #949c82; }
.bg-green { background-color: #5F7A62; }
.bg-brown { background-color: #aa9273; }

@media (max-width: 900px) {
  .news-card, .stats-row { grid-template-columns: 1fr; }
  .news-content { padding: 2rem 1.5rem; }
  .news-content h3 { font-size: 1.5rem; }
  .media-header h2 { font-size: 1.8rem; }
}
</style>
