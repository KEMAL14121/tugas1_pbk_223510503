<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3 style="color: #1E90FF;">IKMAL ARDHIYARO</h3>
  </div>
</template>

<style scoped>
.greetings {
  text-align: center;
  padding: 20px;
  border-radius: 10px;
  background-color: #f8f9fa; /* Warna latar belakang */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Efek bayangan */
  transition: background-color 0.3s; /* Efek transisi */
}

.greetings:hover {
  background-color: #e9ecef; /* Warna latar belakang saat hover */
}

h1 {
  font-weight: 600;
  font-size: 2.6rem;
  color: #198754; /* Warna teks hijau */
  margin-top: 0; /* Menghapus margin atas agar tidak ada jarak berlebih */
}

h3 {
  font-size: 1.2rem;
  color: #6c757d; /* Warna teks abu-abu */
}

.greetings a {
  color: #0d6efd; /* Warna tautan biru */
  text-decoration: none;
}

.greetings a:hover {
  text-decoration: underline; /* Garis bawah saat hover */
}
</style>
