<script lang="ts">
export default {
  name: "ToolsAndProjects",
  components: {},
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
          <a
            title="GitHub"
            href="https://github.com/kaiomaxlira"
            target="_blank"
          >
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
          <a
            title="GitHub"
            href="https://github.com/kaiomaxlira"
            target="_blank"
          >
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
          <a
            title="GitHub"
            href="https://github.com/kaiomaxlira"
            target="_blank"
          >
            <img src="../assets/img/github.svg" alt="Git" class="github" />
          </a>
        </div>
      </div>
    </div>

    <div class="container_tool">
      <span class="tools">Ferramentas</span>

      <div class="container">
        <div class="column">
          <div class="card">
            <a
              href="https://developer.mozilla.org/pt-BR/docs/Web/HTML"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/html5.svg"
                alt="tools"
                title="Html 5"
              />
            </a>
          </div>
          <div class="card">
            <a
              href="https://developer.mozilla.org/pt-BR/docs/Web/CSS"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/css3-alt.svg"
                alt="tools"
                title="Css"
              />
            </a>
          </div>
          <div class="card">
            <a
              href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/js.svg"
                alt="tools"
                title="Java Script"
              />
            </a>
          </div>
          <div class="card">
            <a
              href="https://www.typescriptlang.org/"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/typescript.svg"
                alt="tools"
                title="TypeScript"
              />
            </a>
          </div>
        </div>

        <div class="column">
          <div class="card">
            <a href="https://www.typescriptlang.org/" target="_blank">
              <img
                src="../assets/img/tools_img/tailwind-css.svg"
                alt="tools"
                title="Tailwind Css"
              />
            </a>
          </div>
          <div class="card">
            <a href="https://vuejs.org/" target="_blank">
              <img
                src="../assets/img/tools_img/vuejs.svg"
                alt="tools"
                title="Vuejs"
              />
            </a>
          </div>
          <div class="card">
            <a href="https://react.dev/" target="_blank">
              <img
                src="../assets/img/tools_img/react.svg"
                alt="tools"
                title="React"
              />
            </a>
          </div>
          <div class="card">
            <a
              href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/js.svg"
                alt="tools"
                title="Java Script"
              />
            </a>
          </div>
        </div>

        <div class="column">
          <div class="card">
            <a href="https://laravel.com/" target="_blank">
              <img
                src="../assets/img/tools_img/laravel.svg"
                alt="tools"
                title="Laravel"
              />
            </a>
          </div>

          <div class="card">
            <a href="https://www.python.org/" target="_blank">
              <img
                src="../assets/img/tools_img/python.svg"
                alt="tools"
                title="Python"
              />
            </a>
          </div>

          <div class="card">
            <a
              href="https://www.typescriptlang.org/"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/typescript.svg"
                alt="tools"
                title="TypeScript"
              />
            </a>
          </div>

          <div class="card">
            <a
              href="https://www.typescriptlang.org/"
              target="_blank"
            >
              <img
                src="../assets/img/tools_img/typescript.svg"
                alt="tools"
                title="TypeScript"
              />
            </a>
          </div>
          
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
  gap: 17rem;
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
  border: 1px solid #E6E6E7;
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
  filter: invert(95%) sepia(6%) saturate(23%) hue-rotate(188deg) brightness(98%)
    contrast(91%);
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
  margin-left: 4.7rem;
}

.container {
  display: flex;
  justify-content: space-between;
}

.column {
  display: flex;
  flex-direction: column;
  height: 550px;
}

.card {
  margin: 1.25rem;
  box-sizing: border-box;
  width: 100px;
  height: 100px;
  border: 1px solid white;
  border-radius: 17px;
  cursor: pointer;
  transition: all 0.5s;
  display: flex;
  align-items: center;
  justify-content: center;
}

.card img {
  width: 70px;
  height: 80px;
}

.card:hover {
  border: 1px solid #E6E6E7;
  transform: scale(1.05);
}

.card:active {
  transform: scale(0.95) rotateZ(1.7deg);
}
</style>