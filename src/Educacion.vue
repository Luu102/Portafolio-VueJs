<script setup>
const eventos = [
  { año: "2020 - 2024", titulo: "Secundario Polivalente de Arte", detalle: "Bachiller en Artes orientada a la Pintura" },
  { año: "2025 - Actualidad", titulo: "Tecnicatura Universitaria en Programación", detalle: "Cursando primer año" }
];
</script>

<template>
  <div class="page">
    <div class="card">
      <h1 class="title">Mi Línea del Tiempo Académica</h1>

      <div class="timeline">
        <div
          v-for="(evento, index) in eventos"
          :key="index"
          class="timeline-item"
        >
          <div class="timeline-dot"></div>
          <div class="timeline-content">
            <h2 class="year">{{ evento.año }}</h2>
            <p class="text">{{ evento.titulo }}</p>
            <p class="detail">{{ evento.detalle }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.page {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #131213;
  padding: 20px;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

.card {
  background: rgb(44, 44, 44);
  border-radius: 20px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  padding: 30px;
  max-width: 600px;
  width: 100%;
}

.title {
  text-align: center;
  margin-bottom: 30px;
  font-size: 1.8rem;
  color: #8747da;
}

.timeline {
  position: relative;
  border-left: 3px solid #8747da;
  margin-left: 20px;
  padding-left: 20px;
}

.timeline-item {
  margin-bottom: 25px;
  position: relative;
}

.timeline-dot {
  position: absolute;
  left: -33px;
  top: 5px;
  width: 16px;
  height: 16px;
  background: #28145e;
  border: 3px solid rgb(255, 255, 255);
  border-radius: 50%;
  box-shadow: 0 0 0 2px #28145e;
}

.timeline-content {
  background: #edecee;
  border-radius: 12px;
  padding: 15px 20px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.timeline-content:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 14px rgba(114, 90, 223, 0.76);
}

.year {
  text-align: left;
  font-size: 1.2rem;
  font-weight: bold;
  color: #8747da;
  margin-bottom: 5px;
}

.text {
  font-size: 1rem;
  color: #2b0d53;
  margin: 2px 0;
}

.detail {
  font-size: 0.9rem;
  color: #666;
  font-style: italic;
}
</style>