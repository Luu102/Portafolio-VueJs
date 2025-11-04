<template>
  <section class="seccion-intereses">

    <div
      v-for="(interes, indice) in intereses"
      :key="indice"
      class="card-interes"
    >
      <div class="card-encabezado" @click="alternar(indice)">
        <span class="titulo-card">{{ interes.titulo }}</span>
        <span :class="{'rotada': indiceActivo === indice}">▼</span>
      </div>

      <div v-show="indiceActivo === indice" class="card-contenido">
        <p>{{ interes.descripcion }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const indiceActivo = ref(null)

const intereses = ref([
  {
    titulo: "Diseño de videojuegos",
    descripcion:
      "Me apasiona el proceso de dar vida a ideas interactivas. Me interesa comprender cómo el diseño, la narrativa y la programación se combinan para crear experiencias que conectan emocionalmente con el jugador."
  },
  {
    titulo: "El arte digital",
    descripcion:
      "Considero el arte digital una forma moderna de expresión que combina imaginación y tecnología. Me gusta explorar distintos estilos, técnicas y herramientas digitales para crear imágenes que transmitan sensaciones y reflejen mi visión personal."
  },
  {
    titulo: "Desarrollo de páginas web",
    descripcion:
      "Me gusta diseñar y programar sitios web modernos, funcionales y atractivos. Busco mejorar mis habilidades en front-end y entender cómo crear experiencias visuales intuitivas para los usuarios."
  },
  {
    titulo: "Actividades al aire libre",
    descripcion:
      "Disfruto pasar tiempo al aire libre porque me permite desconectarme del entorno digital y reconectarme con la naturaleza. Valoro la tranquilidad de los paisajes, el sonido del viento y la calidez del sol, que me inspiran y me ayudan a mantener el equilibrio."
  }
])

function alternar(indice) {
  indiceActivo.value = indiceActivo.value === indice ? null : indice
}
</script>

<style scoped>

.seccion-intereses {
  max-width: 700px;
  margin: 60px auto;
  padding: 0 20px;
  font-family: "Poppins", sans-serif;
}


.card-interes {
  border-radius: 12px;
  overflow: hidden;
  margin-bottom: 15px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
  transition: transform 0.2s ease;
}

.card-interes:hover {
  transform: scale(1.01);
}

.card-encabezado {
  background-color: #8747da;
  padding: 18px 20px;
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-weight: bold;
  letter-spacing: 0.5px;
  transition: background-color 0.3s ease;
}

.card-encabezado:hover {
  background-color: #4a148c; 
}

.titulo-card {
  color: aliceblue; 
}

/* Flechita ▼ */
.card-encabezado span.rotada {
  color: #4a148c;
  transition: transform 0.3s ease;
}

/* Contenido  */
.card-contenido {
  background-color: #f3e5f5; 
  color: #4a148c; 
  padding: 18px 20px;
  animation: desplegar 0.3s ease;
  font-size: 0.95rem;
  line-height: 1.6;
}

@keyframes desplegar {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>