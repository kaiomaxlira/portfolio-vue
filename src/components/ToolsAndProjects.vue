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
        <img class="img_p" src="../assets/img/3angulo.png" alt="projeto" />
        <h1>Calcularoda</h1>
        <p>Este projeto tem como função calcular a sua contabilidade no gla</p>
        <button>c</button>
      </div>

      <div class="card_p"></div>
      <div class="card_p"></div>
    </div>

    <div class="container_tool">
      <span class="tools">Ferramentas</span>

      <div class="container">
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
  color: #d3d3d3;
}

/*  Projetos */

.card_p {
  margin: 1rem;
  width: 450px;
  height: 150px;
  box-sizing: border-box;
  border-radius: 17px;
  border: 1px solid white;
  transition: all 0.5s;
  display: flex;
  align-items: self-start;
  justify-content: center;
}

.card_p:hover {
  border: 1px solid #6391ff;
  transform: scale(1.05);
}

.card_p:active {
  transform: scale(0.95) rotateZ(1.7deg);
}

.project {
  margin-left: 9.5rem;
}

.img_p {
  height: 140px;
  width: 140px;
  margin: 0.5rem;
}

.card_p h1 {
  height: 30px;
  width: 140px;
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: italic;
  font-size: 1.5rem;
  color: #d3d3d3;
}

.card_p p {
  margin-top: 2rem;
  margin-right: 1rem;
  font-family: "Poppins", sans-serif;
  font-weight: 100;
  font-style: normal;
  font-size: 0.5rem;
  color: #d3d3d3;
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
  border: 1px solid #6391ff;
  transform: scale(1.05);
}

.card:active {
  transform: scale(0.95) rotateZ(1.7deg);
}

/* .container_project,
.container_tool {
  width: 30rem;
  height: 35rem;
  border-radius: 10% 10% 10% 10%;
  border-right: 0px solid black;
  border-bottom: 0px solid black;
  border-top: 0px solid black;
  border-left: 0px solid black;
  box-shadow: 0 0 10px #6391ff;
} */
</style>
