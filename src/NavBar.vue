<template>
    <nav class="navbar">
      <div class="navbar-menu">
       <ul class="nav-list">
           <li v-for="nav in navegacion" :key="nav.nombre">
                <a :href="nav.enlace" class="nav-item">
                    {{ nav.nombre }}
                </a>
            </li>
       </ul>
      </div>
    </nav>
</template>

<script setup>
import { ref } from "vue";
const navegacion= ref([
    {id:1, nombre:'Educación', enlace:'#educacion'},
    {id:2, nombre:'Experiencia', enlace:'#experiencia'},
    {id:3, nombre:'Proyectos', enlace:'#proyectos'},
    {id:4, nombre:'Habilidades', enlace:'#habilidades'},
    {id:5, nombre:'Intereses', enlace:'#intereses'}
]);
</script>

<style scoped>

.navbar {
  background: linear-gradient(90deg, #330f5c, #a083d4);
  padding: 2rem 2rem;
}

.navbar-menu {
  display: flex;
  justify-content: flex-end;
}

.nav-list {
  display: flex;
  list-style: none;
  gap: 1.5rem; 
  margin: 0;
  padding: 0;
}

.nav-item {
  color: rgb(255, 255, 255);
  text-decoration: none;
}

.nav-item:hover {
  color: rgb(101, 53, 214);
}


a {
  border: 1px solid;
  border-color: hsl(256, 80%, 12%);
  border-radius: 5px;
  text-decoration: none;
  transition: 0.4s;
  padding: 8px;
}

a:hover {
  background-color: hsl(0, 2%, 11%);;
}


/* PARA CELULAR */

@media (max-width: 768px) {
  .nav-list {
    flex-direction: column;    
    align-items: center;
    gap: 1,5rem;
   
  }

  .navbar-menu {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .nav-item {
    font-size: 1rem;
  }
}
</style>