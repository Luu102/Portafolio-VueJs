<script setup>
const title ='Lourdes Eschler';
const descripcion ='Técnico Universitario en Programación - UTN';
const residencia ='San Rafael, Mendoza, Argentina';
const presentacion ='Hola! y bienvienido a mi portafolio. Soy estudiante en la tecnicatura de programación. He aprendido a desarrollar sitios web y algoritmos capaces de solucionar problemas que podemos encontrar en la vida diaria';
const redesSociales = [
    {id:1, name:'linkedin', src:'/src/assets/icons/linkedin_icon.webp', url:'https://www.linkedin.com/in/lourdes-eschler-b0bb9436a/' },
    {id:2, name:'Instagram', src:'/src/assets/icons/instagram_icon.jpg', url:'https://www.instagram.com/lourdes.__7/?next=%2F'},
    {id:3, name:'GitHub', src: '/src/assets/icons/github_icon.png', url: 'https://github.com/Luu102'},
    {id:4, name:'curriculum', src:'/src/assets/icons/curriculum_logo.png', url: ''}
];
const telefono = '+54 9 2604-545304';
</script>



<template>
<section class="datos-personales"></section>
<div class="card">
    <h1>{{ title }}</h1>
    <h2>{{ descripcion }}</h2>
    <p>{{ presentacion }}</p>
    <ul class="container-lista">
      <li v-for="red in redesSociales" :key="red.id">
        <a :href="red.url"><img class="icon-redsocial" :src="red.src" width="35rem" :alt="red.name"></a>
      </li>
    </ul>
    <h3>✆ Mi teléfono personal: {{ telefono }}</h3>
    <h4>{{ residencia }}</h4>
</div>
</template>

<style scoped>
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
  background-color: rgb(142, 212, 133);
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
  box-shadow: 0 0 5px rgb(95, 124, 205, 0.934);
}

.icon-redsocial:hover {
  background-color: rgb(26, 240, 7);
  box-shadow: 0 0 5px rgb(211, 208, 218);
}

h3 {
  font-size: 1.2rem;
  font-weight: 600;
}
</style>