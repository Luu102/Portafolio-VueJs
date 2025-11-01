<script setup>

</script>

<template>
    <div class="proyecto">
  <div class="titulo-proyecto">
    <img src="/src/assets/icons/icon1.svg" alt="" class="icono">
    <h3>Proyecto colaborativo universitario</h3>
  </div>
  <p class="fecha">Marzo 2025 - Diciembre 2027</p>
  <p>Integré un equipo de desarrollo durante mi carrera facultativa en Programación. Participé en el diseño de la base de datos, la implementación del backend en Python y la documentación técnica del proyecto.</p>
</div>

<div class="proyecto">
  <div class="titulo-proyecto">
    <img src="/src/assets/icons/icon2.svg" alt="" class="icono">
    <h3>Proyecto personal de desarrollo web</h3>
  </div>
  <p class="fecha">Mayo 2025 - Julio 2025</p>
  <p>Desarrollé un sitio web interactivo para practicar mis habilidades en HTML, CSS y JavaScript, aplicando principios de diseño responsive y optimización del rendimiento. Implementé funcionalidades dinámicas como formularios validados y componentes reutilizables.</p>
</div>

<div class="proyecto">
  <div class="titulo-proyecto">
    <img src="/src/assets/icons/icon3.svg" alt="" class="icono">
    <h3>Desarrollo de una aplicación de escritorio</h3>
  </div>
  <p class="fecha">Octubre 2025 - Actualidad</p>
  <p>Diseñé y programé una aplicación de escritorio en Java para la gestión de clientes y productos, incorporando una interfaz gráfica y conexión a una base de datos MySQL. El proyecto incluyó funcionalidades de registro, búsqueda y generación de reportes.</p>
</div>
     
</template>

<style scoped>
.titulo-proyecto {
  display: flex;
  align-items: center;
  gap: 10px; /* separa el ícono del texto */
}

.icono {
  width: 30px;
  height: 30px;
}

.proyecto {
  margin-bottom: 40px; /* espacio entre secciones */
}

h3 {
  color: #c38cff; /* tu violeta */
  margin: 0; /* elimina margen por defecto */
  font-weight: bold;
}

.fecha {
  font-style: italic;
  margin-top: 5px;
  color: #ccc;
}

</style>