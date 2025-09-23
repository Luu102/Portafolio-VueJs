<script setup>
import NavBar from './NavBar.vue';
import DatosPersonales from './DatosPersonales.vue';
</script>

<template>
  <header>
    <!--Barra de Navegación-->
    <NavBar />
    <!--Datos Personales-->
    <DatosPersonales />
  </header>
  <main>
    <section id="educacion"><h2>Educación - Cursos</h2></section>
    <section id="experiencia"><h2>Experiencia</h2></section>
    <section id="proyectos"><h2>Proyectos</h2></section>
    <section id="habilidades"><h2>Habilidades</h2></section>
    <section id="intereses"><h2>Intereses</h2></section>
</main>
</template>


<style scoped>

</style>
