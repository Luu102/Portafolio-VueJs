<script setup>

</script>

<template>
    <div class="galeria">
        <div class="proyecto">
            <img src="/src/assets/icons/babushka.png" alt="Proyecto 1">
            <div class="proyecto-info">
                <h3>Identidad gráfica para "Babushka" Panaderia</h3>
                <p>Desarrollo de la línea visual para una panadería artesanal de masa madre. Participé en el proceso de branding, eligiendo paletas de colores, tipografías, y creando logotipos y elementos gráficos para redes sociales y packaging.</p>
            <div class="proyecto-links">
                <a href="https://www.instagram.com/babushkamasamadre/" class="btn-ver-mas" target="_blank" rel="">Ver Proyecto</a>
            </div>
        </div>
        </div>
        <div class="proyecto">
            <img src="/src/assets/icons/unity.png" alt="Proyecto 1">
            <div class="proyecto-info">
                <h3>Videojuego con Unity</h3>
                <p>Proyecto grupal donde colaboré en el diseño visual y la programación básica de un videojuego en 2D. Usamos Unity como motor de desarrollo, y trabajamos en equipo para combinar arte y código en una experiencia interactiva.</p>
            <div class="proyecto-links">
                <a href="" class="btn-ver-mas" target="_blank" rel="">Ver Proyecto</a>
            </div>
        </div>
        </div>
        <div class="proyecto">
            <img src="/src/assets/icons/flask.png" alt="Proyecto 1">
            <div class="proyecto-info">
                <h3>Aplicación web de gestión con Python y Flask</h3>
                <p>Desarrollo de una aplicación web para administrar inventarios y ventas de pequeños comercios. Participé en el diseño del backend con Flask y MySQL, implementando rutas, autenticación de usuarios y conexión con una base de datos. Colaboré en la maquetación del frontend para lograr una interfaz simple y funcional.</p>
            <div class="proyecto-links">
                <a href="" class="btn-ver-mas" target="_blank" rel="">Ver Proyecto</a>
            </div>
        </div>
        </div>
        
    </div>
</template>

<style scoped>

.galeria{
    width: 100%;
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
    justify-content: center;
    background-image: url('/src/assets/icons/fondo.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.proyecto {
    display: flex;
    flex-direction: column;
    border: 2px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    background-color: #f9f9f9;
    max-width: 300px;
    flex: 1 1 300px;
}

.proyecto img {
    width: 100%;          
    height: 200px;        
    object-fit: cover;    
    object-position: center; 
    border-top-left-radius: 8px;
    border-top-right-radius: 8px;
}


.proyecto-info {
    display: flex;
    flex-direction: column;
    padding: 15px;
    text-align: center;
    justify-content: space-between;
    flex: 1; 
}

.proyecto-info h3 {
    margin: 10px 0;
    font-size: 1.3rem;
    color: #333;
}

.proyecto-info p {
    margin: 10px 0;
    font-size: 1em;
    color: #666;
}

.proyecto-links {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: auto;
    text-align: center; /* centra el botón si querés */
}

.proyecto-links .btn-ver-mas {
    background-color: #007BFF;
    color: #fff;
    padding: 10px 15px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0,3s;
}

.proyecto-links .btn-ver-mas:hover {
    background-color: #0056b3;
}

.proyecto-links .github-link {
    color: #333;
    text-decoration: none;
    font-size: 0.9em;
}

.proyecto-links.github-link:hover{
    text-decoration: underline;
}


/* CELULAR */

@media (max-width: 768px) {
  .galeria {         
    padding: 30px 0;
    padding-bottom: 100px;
  }
}
</style>