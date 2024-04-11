<script lang="ts">
export default {
  components: {},
};
</script>

<template>
  <div class="aboutme">
    <div class="container">
      <div class="title_content">
        Sobre
        <div class="content">
          Formado em Sistemas de Informações com algumas experiências em estagio e freelancer acumulei
          conhecimentos nas areas de QA (Controle de qualidade) front-ende e back-end, onde desenvolvir minhas habilidades
          com react, vue, tailwind css, php, laraval e cypress. Com isto tenho a capacidade de criar intefaces web,
          APIS rest e fazer testes de qualidade. Com a mente aberta para inovação e um compromisso inabalável com a qualidade,
          estou pronto para criar soluções que inspirem, encantem e façam a diferença no universo da web. 
        </div>
      </div>
      <div class="title_information">Informações
      <div class="my_informations">
        <div class="info">
          <span class="label">Idade:</span>
          <span class="value">23 anos</span>
        </div>
        <div class="info">
          <span class="label">Email:</span>
          <span class="value">kaiomaxlira@outlook.com</span>
        </div>
        <div class="info">
          <span class="label">Telefone:</span>
          <span class="value">+55 (88) x xxxx-xxxx</span>
        </div>
        <div class="info">
          <span class="label">Linguagem:</span>
          <span class="value">Português, English</span>
        </div>
        <div class="info">
          <span class="label">Localização:</span>
          <span class="value">Aurora, Ceará, Brasil</span>
        </div>
      </div>
      </div>
    </div>
    <img class="backimg" src="../assets/img/background.jpg" alt="background" />
  </div>
</template>

<style scoped>
.aboutme {
  margin: 0;
  width: 100%;
  height: 615px;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

}

.container {
  width: 73rem;
  height: 28rem;
  background-color: #d9d9d9;
  border-radius: 0px 50px 0px 50px;
  position: relative;
  display: flex;
}

.title_content {
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
  font-size: 2.5rem;
  color: rgb(43, 41, 41);
  margin-top: 4rem;
  margin-left: 5rem;
}

.content {
  margin-right: 0.5rem;
  font-weight: 500;
  font-size: 1rem;
  color: rgb(43, 41, 41);
  width: 40rem;
  margin-top: 2rem;
  line-height: 1.5rem;
}

.title_information {
  font-family: "Poppins", sans-serif;
  font-weight: 900;
  font-size: 2rem;
  font-size: 2.5rem;
  color: rgb(43, 41, 41);
  margin-top: 4rem;
  margin-left: 4rem;
}
.my_informations {
  display: flex;
  line-height: 2.5rem;
  flex-direction: column;
  margin-top: 1rem;
}

.info {
  display: flex; /* Exibe os itens em linha */
  margin-bottom: 0.1rem; /* Espaçamento entre os itens */
}

.label {
  margin-right: 0.5rem;
  font-weight: 700;
  color: rgb(43, 41, 41);
  font-size: 1.1rem;
}

.value {
  margin-right: 0.5rem;
  font-weight: 500;
  font-size: 1rem;
  color: rgb(43, 41, 41);
}

.backimg {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  object-fit: contain;
  object-fit: cover;
  z-index: -1;
}
</style>