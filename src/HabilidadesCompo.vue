<script setup>
</script>

<template>
    <div class="skills-contenedor">
        <div class="skills-categoria">
            <h3>Lenguaje de Programación</h3>
            <ul class="skills">
                <li class="skill">
                    <img src="/src/assets/icons/javascript.svg.svg" alt="JavaScript">
                    <span>JavaScript: Avanzado</span>
                </li>
                <li class="skill">
                    <img src="/src/assets/icons/python.svg.svg" alt="Python">
                    <span>Python: Intermedio</span>
                </li>
                <li class="skill">
                    <img src="/src/assets/icons/html.svg.svg" alt="">
                    <span>HTML/CSS: Avanzado</span>
                </li>
                <li class="skill">
                    <img src="/src/assets/icons/java.svg.svg" alt="">
                    <span>Java: Intermedio</span>
                </li>
                <li class="skill">
                    <img src="/src/assets/icons/sql.svg" alt="SQL">
                    <span>SQL: Intermedio</span>
                </li>
            </ul>
        </div>
    <div class="skills-categoria">
        <h3>Frameworks y Librerías</h3>
        <ul class="skills">
            <li class="skill">
                <img src="/src/assets/icons/react-js.png" alt="React.js">
                <span>React.js: Avanzado</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/Vue.svg" alt="Vue.js">
                <span>Vue.js: Intermedio</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/node-js.svg" alt="Node.js">
                <span>Node.js: Avanzado</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/django.svg" alt="Django">
                <span>Django: Intermedio</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/bootstrap.svg" alt="Bootstrap">
                <span>Bootstrap: Avanzado</span>
            </li>
        </ul>
    </div>

    <div class="skills-categoria">
        <h3>Herramientas y Software</h3>
        <ul class="skills">
            <li class="skill">
                <img src="/src/assets/icons/git.svg" alt="Git">
                <span>Git: Avanzado</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/docker.svg" alt="Docker">
                <span>Docker: Intermedio</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/cypress.svg" alt="Cypress">
                <span>Cypress: Intermedio</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/figma.svg" alt="Figma">
                <span>Figma: Intermedio</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/visual-studio-code.svg" alt="Visual Studio Code">
                <span>Visual Studio Code: Avanzado</span>
            </li>
        </ul>
    </div>

    <div class="skills-categoria">
        <h3>Bases de Datos</h3>
        <ul class="skills">
            <div class="skill">
                <img src="/src/assets/icons/mongodb.svg" alt="MongoDB">
                <span>MongoDB: Avanzado</span>
            </div>
            <div class="skill">
                <img src="/src/assets/icons/mysql.svg" alt="MySQL">
                <span>MySQL: Intermedio</span>
            </div>
            <div class="skill">
                <img src="/src/assets/icons/postgresql.svg" alt="PostgreSQL">
                <span>PostgreSQL: Intermedio</span>
            </div>
        </ul>
    </div>

    <div class="skills-categoria">
        <h3>Idiomas</h3>
        <ul class="skills">
            <li class="skill">
                <img src="/src/assets/icons/arg.svg" alt="Arg">
                <span>Español: Nativo</span>
            </li>
            <li class="skill">
                <img src="/src/assets/icons/eeuu.png" alt="EEUU">
                <span>Inglés: Intermedio (B2)</span>
            </li>
        </ul>
    </div>
    </div>
</template>

<style scoped>
.skills-contenedor {
    padding: 2rem;
}

.skills-categoria {
    margin-bottom: 20px;
}

.skills-categoria h3 {
    display: flex;
    justify-content: left;
    margin-bottom: 10px;
    font-size: 1.5em;
    color: #8747da;
    font-size: 1.5em;
    font-weight: bold;
}

.skills {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    gap: 20px;
}

.skill {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    background-color:aliceblue;
    padding: 0.3em;
    border-radius: 8px;
    box-shadow: 0px 4 px 12px rgba(52, 13, 102, 0.963);
    flex: 1 1 200px;
    max-width: 250px;
}

.skill:hover {
    background-color: rgba(114, 90, 223, 0.76);
}

.skill img {
    width: 35px;
    height: 35px;
}

.skill span {
    font-size: 1em;
    color: #333333;
}

.skill:hover {
    font-size: 1.3em;
    transition: 2s ease;
}
@media (max-width: 768px) {
    .skills-categoria h3 {
        justify-content: center;
    }

    .skill {
        justify-content: center;
    }
}

</style>
