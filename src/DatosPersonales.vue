<script setup>
import linkedin from '/src/assets/icons/linkedin_icon.webp'
import instagram from '/src/assets/icons/instagram_icon.jpg'
import github from '/src/assets/icons/github_icon.png'
import cv from '/src/assets/icons/curriculum_logo.png'

import FondoLava from './FondoLava.vue';
const title ='Lourdes Eschler';
const descripcion ='Técnico Universitario en Programación - UTN';
const residencia ='San Rafael, Mendoza, Argentina';
const presentacion ='Hola! y bienvienido a mi portafolio. Soy estudiante en la tecnicatura de programación. He aprendido a desarrollar sitios web y algoritmos capaces de solucionar problemas que podemos encontrar en la vida diaria';
const redesSociales = [
    {id:1, name:'linkedin', src:linkedin, url:'https://www.linkedin.com/in/lourdes-eschler-b0bb9436a/' },
    {id:2, name:'Instagram', src:instagram, url:'https://www.instagram.com/lourdes.__7/?next=%2F'},
    {id:3, name:'GitHub', src:github, url: 'https://github.com/Luu102'},
    {id:4, name:'curriculum', src:cv, url: ''}
];
const telefono = '+54 9 2604-545304';
</script>

<template>
  <section class="datos-personales">
    <div class="tarjeta">
      <!-- Fondo animado -->
      <div class="fondo-lava">
        <FondoLava />
      </div>

      <!-- Contenido -->
      <div class="contenido">
        <h1>{{ title }}</h1>
        <h2>{{ descripcion }}</h2>
        <p>{{ presentacion }}</p>

        <ul class="container-lista">
          <li v-for="red in redesSociales" :key="red.id">
            <a :href="red.url" target="_blank">
              <img class="icon-redsocial" :src="red.src" width="35rem" :alt="red.name" />
            </a>
          </li>
        </ul>

        <h3>✆ Mi teléfono personal: {{ telefono }}</h3>
        <h4>{{ residencia }}</h4>
      </div>
    </div>
  </section>
</template>


<style scoped>

.telefono {
  color: aliceblue;
}

.h3 {
  color: aliceblue;
}

.tarjeta {
  position: relative;
  border-radius: 15px;
  padding: 40px;
  max-width: 800px;
  margin: 50px auto;
  overflow: hidden; /* mantiene el fondo dentro del borde */
}

/* Fondo animado */
.fondo-lava {
  position: absolute;
  inset: 0;
  z-index: 0;
  opacity: 0.35; /* controlá la intensidad */
}

/* Contenido encima del fondo */
.contenido {
  position: relative;
  z-index: 1;
  color: white;
  text-align: center;
}


.page {
  min-height: 100vh;
  background: #131213;
  padding: 20px;
}

ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 1rem;
  padding: 0;
}

ul li {
  display: inline-block;
}
h1 {
  font-size: 2.5rem;
}

p {
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.card {
  background-color:  transparent;
  border-radius: 10px;
  padding: 20px;
  margin: 50px;
  text-align: center;
}

.icon-redsocial {
  align-items: flex;
  background-color: aliceblue;
  border-radius: 50%;
  padding: 2px;
  margin: 5px;
  box-shadow: 0 0 5px rgba(115, 95, 205, 0.934);
}

.icon-redsocial:hover {
  background-color:  rgba(114, 90, 223, 0.76);
  box-shadow: 0 0 5px rgb(211, 208, 218);
}

h3 {
  font-size: 1.2rem;
  font-weight: 600;
}

/* CELULAR */
@media (max-width: 768px) {
  .card {
    display: flex;
    flex-direction: column;
    width: 95%;
    max-width: 380px;
    padding: 25px 15px;
    justify-content: center;
  }

  .card h1 {
    font-size: 1.8rem;
  }

  .card h2 {
    font-size: 1.1rem;
  }

  .card p {
    font-size: 0.95rem;
  }
}

</style>