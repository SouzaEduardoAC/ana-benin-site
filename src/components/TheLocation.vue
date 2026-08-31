<script setup lang="ts"></script>

<template>
  <section class="location-section" id="localizacao">
    <div class="container">
      <div class="location-title">
        <small class="loc-subtitle">LOCAL DE ATENDIMENTO</small>
        <h2>Você no Centro do Cuidado</h2>
        <p class="loc-desc">
          Ambiente acolhedor e moderno, pensado para o seu conforto.
        </p>
      </div>

      <div class="location-grid">
        <div class="loc-info-col">
          <div class="info-card">
            <div class="meso-logo-placeholder">
              <h3 class="meso-title">CR7 Alameda Business</h3>
              <p class="meso-desc">
                Centro empresarial e médico em Blumenau, com infraestrutura
                moderna e confortável.
              </p>
            </div>
          </div>

          <div class="info-card-grid">
            <div class="info-card">
              <div>
                <h4>Ambiente Seguro</h4>
                <p class="card-subtext">Protocolos sanitários rigorosos</p>
              </div>
            </div>
            <div class="info-card">
              <div>
                <h4>Equipe Dedicada e Interdisciplinar</h4>
                <p class="card-subtext">Atendimento humanizado</p>
              </div>
            </div>

            <div class="info-card">
              <div>
                <h4>Estacionamento</h4>
                <p class="card-subtext">Facilidade de acesso</p>
              </div>
            </div>
            <div class="info-card">
              <div>
                <h4>Tecnologias Aprovadas</h4>
                <p class="card-subtext">Conforme orgãos regulatórios</p>
              </div>
            </div>
          </div>

          <div class="address-card">
            <h3><i class="fa-solid fa-location-dot"></i> Endereço</h3>
            <p class="addr-text">
              <strong>CR7 Alameda Business</strong><br />
              R. Hermann Huscher, 113, sala 209<br />
              Vila Formosa - Blumenau - SC, 89023-000
            </p>
            <hr class="addr-divider" />
            <ul>
              <li>
                <i class="fa-solid fa-phone"></i> Entre em contato para agendar:
                (47) 93388-3134
              </li>
              <li>
                <i class="fa-regular fa-clock"></i> Segunda às sexta, 8h às 18h
              </li>
            </ul>
          </div>
        </div>

        <div class="map-col">
          <div class="map-frame">
            <iframe
              src="https://maps.google.com/maps?q=CR7+Alameda+Business,+Rua+Hermann+Huscher,+113+-+Vila+Formosa,+Blumenau+-+SC,+89023-000&amp;t=&amp;z=16&amp;ie=UTF8&amp;iwloc=&amp;output=embed"
              width="600"
              height="450"
              style="border: 0"
              allowfullscreen="false"
              class="map-iframe"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
            ></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.location-section {
  background-color: var(--bg-beige);
  padding: 4rem 0;
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.location-title {
  text-align: center;
  margin-bottom: 3rem;
}
.location-title h2 {
  font-size: 2.5rem;
  color: #222;
}

.loc-subtitle {
  color: #777;
  font-weight: 700;
}
.loc-desc {
  color: #666;
}

.location-grid {
  display: grid;
  grid-template-columns: 0.8fr 1.2fr;
  gap: 2rem;
}

.loc-info-col {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.info-card-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

.info-card {
  background: white;
  padding: 1.5rem;
  border-radius: 12px;
  display: flex;
  gap: 15px;
  align-items: flex-start;
}

.meso-logo-placeholder {
  width: 100%;
  height: auto;
  background: white;
  display: block;
  padding: 0;
}
.meso-title {
  color: #333;
  margin-bottom: 5px;
}
.meso-desc {
  font-size: 0.9rem;
  color: #666;
}

.icon-box {
  width: 40px;
  height: 40px;
  border-radius: 6px;
  flex-shrink: 0;
}
.bg-beige-icon {
  background: #d6cfc4;
}
.bg-green-icon {
  background: #526f4f;
}

.card-subtext {
  font-size: 0.85rem;
  color: #666;
}

.address-card {
  background: #79591f;
  color: white;
  padding: 2rem;
  border-radius: 12px;
  margin-top: 1rem;
}
.address-card h3 {
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  gap: 10px;
}
.address-card ul li {
  display: flex;
  gap: 10px;
  margin-bottom: 10px;
  font-size: 0.9rem;
  opacity: 0.9;
}

.addr-text {
  margin-bottom: 1rem;
}
.addr-divider {
  border: 0;
  border-top: 1px solid rgba(255, 255, 255, 0.2);
  margin: 15px 0;
}

.btn-address {
  width: 100%;
  background: #b0a08b;
  color: #333;
  margin-top: 1rem;
}

.map-col {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.map-frame {
  background-color: #eee;
  border-radius: 12px;
  height: 100%;
  width: 100%;
  overflow: hidden;
  position: relative;
}
.map-iframe {
  width: 100%;
  height: 100%;
  border: 0;
}

.team-img {
  height: 250px;
  border-radius: 12px;
  background: url("https://images.unsplash.com/photo-1631217868264-e5b90bb7e133?q=80&w=2691&auto=format&fit=crop")
    center/cover;
  position: relative;
  display: flex;
  align-items: flex-end;
  padding: 1rem;
}
.team-caption {
  color: white;
  font-size: 0.9rem;
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.8);
}

@media (max-width: 900px) {
  .location-grid {
    grid-template-columns: 1fr;
  }
  .location-section {
    padding: 4rem 0;
  }
  .location-title h2 {
    font-size: 2.2rem;
  }
  .info-card-grid {
    grid-template-columns: 1fr;
  }
}
</style>
