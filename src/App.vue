<script setup>
import Experiencia from './ExperienciaCompo.vue'
import NavBar from './NavBar.vue';
import DatosPersonales from './DatosPersonales.vue';
import Educacion from './Educacion.vue';
import HabilidadesCompo from './HabilidadesCompo.vue';
import ExperienciaCompo from './ExperienciaCompo.vue';
import InteresesCompo from './InteresesCompo.vue';
import ProyectoCompo from './ProyectoCompo.vue';
</script>

<template>
  <header>
    <!--Barra de Navegación-->
    <NavBar />
    <!--Datos Personales-->
    <DatosPersonales />
  </header>
  <main>
    <section id="educacion"><h2>Educación - Cursos</h2>
    <Educacion />
    </section>
    <section id="experiencia"><h2>Experiencia</h2></section>
    <ExperienciaCompo />
    <section id="proyectos"><h2>Proyectos</h2></section>
    <ProyectoCompo />
    <section id="habilidades"><h2>Habilidades</h2></section>
    <HabilidadesCompo />
    <section id="intereses"><h2>Intereses</h2></section>
    <InteresesCompo />

    <footer>
      <a href="#top">Inicio</a>
      <p> @ 2025 Lourdes Eschler - Portafolio web </p>
    </footer>

</main>
</template>


<style scoped>
footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
  font-size: 1.3rem;
}

footer a:hover {
  color: blueviolet;
}

/* CELULAR */

@media (max-width: 768px) {
  footer p {
    justify-content: center;
    font-size: small;
  }
}


</style>
