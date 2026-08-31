<script setup lang="ts">
import logoUrl from "@/assets/logo_no_background.png";
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img :src="logoUrl" alt="AB Neuro Logo" class="logo-img" /> Dra. Ana
        Benin
      </div>
      <nav>
        <ul>
          <li><a href="#sobre">Sobre</a></li>
          <!-- <li><a href="#servicos">Serviços</a></li> -->
          <li><a href="#localizacao">Localização</a></li>
          <li><a href="#contato">Contato</a></li>
        </ul>
      </nav>
      <!-- <a href="#" class="btn btn-primary">Agendar Consulta</a> -->
    </div>
  </header>
</template>

<style scoped>
header {
  position: absolute;
  top: 0;
  width: 100%;
  z-index: 100;
  padding: 1.5rem 0;
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.7), transparent);
}

header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  font-size: 1.5rem;
  font-weight: 700;
  color: #a68e76;
}

.logo-img {
  height: 60px;
  width: auto;
  margin-right: 10px;
}

nav ul {
  display: flex;
  gap: 2rem;
}
nav a {
  color: #ddd;
  font-size: 0.9rem;
  font-weight: 500;
}
nav a:hover {
  color: white;
}

@media (max-width: 900px) {
  nav ul {
    display: none;
  }
  .logo-img {
    height: 45px;
  }
  header {
    padding: 0.8rem 0;
  }
  .logo {
    font-size: 1.1rem;
  }
}
</style>
