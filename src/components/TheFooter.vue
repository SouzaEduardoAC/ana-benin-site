<script setup lang="ts">
import logoUrl from "@/assets/logo_no_background.png";
</script>

<template>
  <footer class="footer-cta" id="contato">
    <div class="container">
      <div class="footer-links">
        <div class="f-col">
          <div class="logo-footer">
            <img :src="logoUrl" alt="AB Neuro Logo" class="logo-img" /> Dra. Ana
            Benin
          </div>
          <p class="f-desc">
            Neurologia e Medicina Interna com visão integral da sua saúde em
            Blumenau.
          </p>
          <div class="social-icons">
            <a
              href="https://www.instagram.com/anabenin.neuro"
              target="_blank"
              class="social-btn"
              ><i class="fa-brands fa-instagram"></i
            ></a>
            <a
              href="https://www.linkedin.com/in/ana-caroline-benin-8ba4839a/"
              target="_blank"
              class="social-btn"
              ><i class="fa-brands fa-linkedin-in"></i
            ></a>
            <a
              href="https://wa.me/5547933883134"
              target="_blank"
              class="social-btn"
              ><i class="fa-brands fa-whatsapp"></i
            ></a>
          </div>
        </div>

        <div class="f-col">
          <h4>Links Rápidos</h4>
          <ul>
            <li><a href="#">> Home</a></li>
            <li><a href="#sobre">> Sobre</a></li>
            <!-- <li><a href="#servicos">> Serviços</a></li> -->
            <li><a href="#localizacao">> Localização</a></li>
            <li><a href="#contato">> Contato</a></li>
          </ul>
        </div>
        <!-- 
        <div class="f-col">
          <h4>Especialidades</h4>
          <ul>
            <li><i class="fa-solid fa-check"></i> Neurologia Geral</li>
            <li><i class="fa-solid fa-check"></i> Tratamento de Cefaleias</li>
            <li><i class="fa-solid fa-check"></i> Neurointensivismo</li>
            <li><i class="fa-solid fa-check"></i> Medicina Interna</li>
            <li><i class="fa-solid fa-check"></i> Formação Albert Einstein</li>
          </ul>
        </div> -->

        <div class="f-col">
          <h4>Contato</h4>
          <ul>
            <li>
              <i class="fa-solid fa-location-dot"></i> R. Hermann Huscher, 113,
              sala 209<br />Vila Formosa, Blumenau - SC
            </li>
            <li><i class="fa-solid fa-building"></i> CR7 Alameda Business</li>
            <li><i class="fa-solid fa-phone"></i> (47) 93388-3134</li>
          </ul>
          <a
            href="https://wa.me/5547933883134"
            class="btn btn-small"
            target="_blank"
            ><i class="fa-brands fa-whatsapp"></i> Agendar Minha Consulta</a
          >
        </div>
      </div>

      <div class="copyright">
        <div>© 2025 Dra. Ana Caroline Benin. Todos os direitos reservados.</div>
        <div class="legal-links">
          <a href="#">Política de Privacidade</a>
          <a href="#">Termos de Uso</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer-cta {
  background-color: var(--bg-dark-green);
  background-image: radial-gradient(#4a574e 1px, transparent 1px);
  background-size: 20px 20px;
  padding: 5rem 0 2rem;
  color: #ccc;
  text-align: center;
}

.final-cta h2 {
  color: #dacba9;
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
}
.final-cta h2 span {
  color: #f0f0f0;
}
.final-cta p {
  max-width: 600px;
  margin: 0 auto 3rem;
}

.icon-circle {
  width: 60px;
  height: 60px;
  background: #b0a08b;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 20px;
  color: #333;
  font-size: 1.5rem;
}

.footer-cards {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  margin-bottom: 3rem;
}
.f-card {
  background: rgba(140, 120, 103, 0.4);
  padding: 2rem;
  border-radius: 8px;
  border: 1px solid rgba(140, 120, 103, 0.6);
  width: 250px;
}
.f-card i {
  font-size: 2rem;
  color: #ddd;
  margin-bottom: 10px;
  display: block;
}
.f-card h4 {
  color: white;
  font-size: 0.95rem;
  margin-bottom: 5px;
}
.f-card span {
  font-size: 0.75rem;
  color: #ccc;
}

.cta-group {
  justify-content: center;
  margin-bottom: 3rem;
  display: flex;
  gap: 1rem;
}
.btn-brown {
  background: #b0a08b;
  color: #222;
}
.btn-transparent {
  background: transparent;
  border: 1px solid white;
  color: white;
}

.footer-links {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  text-align: left;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  padding-top: 3rem;
  margin-top: 3rem;
}

.f-col h4 {
  color: white;
  margin-bottom: 1.5rem;
}
.f-col ul li {
  margin-bottom: 0.8rem;
  font-size: 0.9rem;
}
.f-col ul li i {
  color: #888;
  margin-right: 8px;
  width: 15px;
}
.f-col ul li a {
  color: #ccc;
}
.f-col ul li a:hover {
  color: white;
}

.logo-footer {
  display: flex;
  align-items: center;
  font-weight: 700;
  color: #a68e76;
  margin-bottom: 1rem;
}
.logo-img {
  height: 50px;
  width: auto;
  margin-right: 10px;
}
.f-desc {
  font-size: 0.85rem;
  color: #999;
  line-height: 1.6;
  margin-bottom: 1rem;
}

.social-icons {
  display: flex;
  gap: 10px;
  margin-top: 1rem;
}
.social-btn {
  width: 35px;
  height: 35px;
  background: rgba(255, 255, 255, 0.1);
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  color: #aaa;
}
.social-btn:hover {
  background: var(--primary-green);
  color: white;
}

.btn-small {
  background: #526f4f;
  width: 100%;
  padding: 10px;
  font-size: 0.9rem;
  color: white;
}

.copyright {
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  margin-top: 2rem;
  padding-top: 1.5rem;
  display: flex;
  justify-content: space-between;
  font-size: 0.8rem;
}

.legal-links {
  display: flex;
  gap: 20px;
}
.legal-links a {
  color: #ccc;
}

@media (max-width: 900px) {
  .footer-links,
  .footer-cards {
    grid-template-columns: 1fr;
    flex-direction: column;
  }
  .f-card {
    width: 100%;
  }
}
</style>
