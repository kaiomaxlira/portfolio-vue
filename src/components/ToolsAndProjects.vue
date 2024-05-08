<script lang="ts">

import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: "ToolsAndProjects",
  components: {
    FontAwesomeIcon,
  },
};
</script>

<template>
  <div class="ToolsAndProjects">
    <div class="container_project">
      <span class="project">Projetos</span>

      <div class="card_p">
        <a href="https://github.com/kaiomaxlira" target="_blank">
          <img   
            src="../assets/img/mago.jpg"
            alt="projeto"
            title="Calculadora na web"
            class="img_p"
          />
        </a>
        <div>
          <h1>Calcularoda</h1>
          <p>
            Este projeto tem como função calcular a <br />sua contabilidade no
            gla
          </p>
        </div>
        <div class="link_projeto">
          <a title="GitHub" href="https://github.com/kaiomaxlira" target="_blank">
            <img src="../assets/img/github.svg" alt="Git" class="github" />
          </a>
        </div>
      </div>

      <div class="card_p">
        <a href="https://github.com/kaiomaxlira" target="_blank">
          <img   
            src="../assets/img/mago.jpg"
            alt="projeto"
            title="Calculadora na web"
            class="img_p"
          />
        </a>
        <div>
          <h1>Calcularoda</h1>
          <p>
            Este projeto tem como função calcular a <br />sua contabilidade no
            gla
          </p>
        </div>
        <div class="link_projeto">
          <a  title="GitHub" href="https://github.com/kaiomaxlira" target="_blank">
            <img src="../assets/img/github.svg" alt="Git" class="github" />
          </a>
        </div>
      </div>

      <div class="card_p">
        <a href="https://github.com/kaiomaxlira" target="_blank">
          <img   
            src="../assets/img/mago.jpg"
            alt="projeto"
            title="Calculadora na web"
            class="img_p"
          />
        </a>
        <div>
          <h1>Calcularoda</h1>
          <p>
            Este projeto tem como função calcular a <br />sua contabilidade no
            gla
          </p>
        </div>
        <div class="link_projeto">
          <a  title="GitHub" href="https://github.com/kaiomaxlira" target="_blank">
            <img src="../assets/img/github.svg" alt="Git" class="github" />
          </a>
        </div>
      </div>
    </div>

    <div class="container_tool">
      <span class="tools">Ferramentas</span>

      <div class="container">
        <div class="column">
          <div class="card"><font-awesome-icon icon="laravel" /></div>
          <div class="card">Click me</div>
          <div class="card">Click me</div>
        </div>

        <div class="column">
          <div class="card">Click me</div>
          <div class="card">Click me</div>
          <div class="card">Click me</div>
        </div>

        <div class="column">
          <div class="card">Click me</div>
          <div class="card">Click me</div>
          <div class="card">Click me</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.ToolsAndProjects {
  margin: 0;
  margin-top: 2rem;
  width: 100%;
  height: 615px;
  display: flex;
  gap: 15rem;
  align-items: flex-start;
  justify-content: center;
}

.ToolsAndProjects span {
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
  font-size: 2.5rem;
  color: #989c90;
}

/*  Projetos */

.card_p {
  margin: 1rem;
  width: 450px;
  height: 150px;
  box-sizing: border-box;
  border-radius: 17px;
  border: 1px solid #989c90;
  transition: all 0.5s;
  display: flex;
  align-items: self-start;
  justify-content: space-between;
}

.card_p:hover {
  border: 1px solid #bc6c64;
  transform: scale(1.05);
}

.card_p:active {
  transform: scale(0.95) rotateZ(1.7deg);
}

.project {
  margin-left: 9.5rem;
}

.img_p {
  height: 130px;
  width: 130px;
  margin: 0.5rem;
  margin-left: 1rem;
  cursor: pointer;
  border-radius: 10%;
  transition: transform 0.3s;
}

.img_p:hover {
  transform: scale(1.05);
}

.link_projeto {
  margin-top: 3.5rem;
  margin-right: 1rem;
}

.github a img {
  width: 2.1rem;
}

.github {
  height: 2rem;
  margin: 0rem;
  width: 1.5rem;
  transition: transform 0.3s ease-in-out;
}

.github:hover {
  filter: invert(95%) sepia(6%) saturate(23%) hue-rotate(188deg) brightness(98%) contrast(91%);
  transform: scale(1.09);
}

.card_p h1 {
  height: 30px;
  width: 140px;
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: italic;
  font-size: 1.5rem;
  color: #989c90;
  margin-top: 0.3rem;
}

.card_p p {
  margin-top: 1rem;
  margin-right: 2rem;
  font-family: "Poppins", sans-serif;
  font-weight: 100;
  font-style: normal;
  font-size: 0.6rem;
  color: #989c90;
}

/* Ferramentas */

.tools {
  margin-left: 4rem;
}

.container {
  display: flex;
  justify-content: space-between;
}

.column {
  display: flex;
  flex-direction: column;
}

.card {
  margin: 1.25rem;
  box-sizing: border-box;
  width: 100px;
  height: 100px;
  border: 1px solid white;
  box-shadow: 12px 17px 51px rgba(0, 0, 0, 0.22);
  backdrop-filter: blur(6px);
  border-radius: 17px;
  text-align: center;
  cursor: pointer;
  transition: all 0.5s;
  display: flex;
  align-items: center;
  justify-content: center;
  user-select: none;
  font-weight: bolder;
  color: black;
}

.card:hover {
  border: 1px solid #bc6c64;
  transform: scale(1.05);
}

.card:active {
  transform: scale(0.95) rotateZ(1.7deg);
}

</style>