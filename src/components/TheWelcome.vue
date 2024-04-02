<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'

import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <div class="welcome-container">
    <!-- WelcomeItem pertama -->
    <WelcomeItem class="welcome-item">
      <template #icon>
        <DocumentationIcon />
      </template>
      <template #heading>DATA DIRI</template>

      NAMA : IKMAL ARDHIYARO
      <h4>NPM : 223510503</h4>
      <h4>MATKUL : PRAKTIKUM PBK</h4>
    </WelcomeItem>

    <!-- WelcomeItem kedua -->
    <WelcomeItem class="welcome-item">
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>KEAHLIAN</template>
      ~PENGAMAT
      <h4>~BERDIKUSI</h4>
      <h4>~HTML</h4>
      <h4>~CSS</h4>
      <h4>~JS</h4>
    </WelcomeItem>

    <!-- WelcomeItem ketiga -->
    <WelcomeItem class="welcome-item">
      <template #icon>
        <EcosystemIcon />
      </template>
      <template #heading>TENTANG SAYA</template>
      Saya bersusia 21 tahun, pengalaman saya pernah menjadi kepala sebuah perkantoran yang berbasis
      perekonomian daerah , dan pengalaman lainnya menjadi wartawan sebuah stasiun televisi
    </WelcomeItem>

    <!-- WelcomeItem empat -->
    <WelcomeItem class="welcome-item">
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>KONTAK</template>

      no hp : 085179714126
      <h4>email : ikmalardhiyaro012@gmail.com</h4>
    </WelcomeItem>
  </div>
</template>
<style scoped>
.welcome-item {
  display: flex;
  flex-direction: column;
  padding: 20px;
  border-radius: 10px;
  background-color: #ffffff; /* Warna latar belakang */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Efek bayangan */
  transition:
    transform 0.3s ease,
    background-color 0.3s ease; /* Efek transisi */
}

/* Efek hover */
.welcome-item:hover {
  transform: translateY(-5px); /* Efek angkat saat hover */
  background-color: #f0f0f0; /* Warna latar belakang saat hover */
}

.welcome-item a {
  color: #3182ce; /* Warna tautan */
  text-decoration: none;
}

.welcome-item a:hover {
  text-decoration: underline; /* Garis bawah saat hover */
}

.welcome-item code {
  background-color: #edf2f7; /* Warna latar belakang untuk kode */
  padding: 2px 4px;
  border-radius: 4px;
}
</style>

<style scoped>
.welcome-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); /* Atur grid untuk responsif */
  gap: 20px; /* Jarak antara item */
}

.welcome-item {
  display: flex;
  flex-direction: column;
  padding: 20px;
  border-radius: 10px;
  background-color: #ffffff; /* Warna latar belakang */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Efek bayangan */
  transition: transform 0.3s ease;
}

.welcome-item:hover {
  transform: translateY(-5px); /* Efek angkat saat hover */
}

.welcome-item a {
  color: #3182ce; /* Warna tautan */
  text-decoration: none;
}

.welcome-item a:hover {
  text-decoration: underline; /* Garis bawah saat hover */
}

.welcome-item code {
  background-color: #edf2f7; /* Warna latar belakang untuk kode */
  padding: 2px 4px;
  border-radius: 4px;
}
</style>
