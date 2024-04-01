<script lang="ts">
export default {
  data() {
    return {
      kaioVisible: false, // Alterado para false
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
    this.handleScroll(); // Chamada inicial para verificar a visibilidade do elemento KAIO
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const scrollPosition = window.scrollY || window.pageYOffset;
      // Define um limite de rolagem para mostrar o elemento Kaio
      const scrollThreshold = 200; // ajuste conforme necessário
      // Verifica se a rolagem ultrapassou o limite e se o KAIO ainda não está visível
      if (scrollPosition >= scrollThreshold && !this.kaioVisible) {
        this.kaioVisible = true; // Define kaioVisible como true para mostrar o elemento KAIO
      } else if (scrollPosition < scrollThreshold && this.kaioVisible) {
        this.kaioVisible = false; // Define kaioVisible como false para ocultar o elemento KAIO
      }
    },
  },
};
</script>

<template>
  <body>
    <div class="logo" ref="container">
      <span :class="{ 'kaio': kaioVisible, 'kaio-animation': !kaioVisible }">KAIO</span>
      <img class="logo-img" src="../assets/img/kaio.png" alt="logo" />
      <span class="max">MAX</span>
    </div>
  </body>
</template>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 9rem;
  margin-top: 10rem;
}

.logo {
  height: 210px;
  width: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.logo-img {
  opacity: 0;
  animation: zoomIn 4s forwards;
}

@keyframes zoomIn {
  from {
    transform: scale(0); 
    opacity: 0; 
  }
  to {
    transform: scale(1); 
    opacity: 1; 
  }
}

.kaio {
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  opacity: 0;
  animation: slideInLeft 3s forwards;
}

@keyframes slideInLeft {
  from {
    transform: translateX(-100%);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

.kaio-animation {
  transition: opacity 0.5s ease;
  opacity: 0;
}

.max {
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  margin-left: 12px;
  opacity: 0;
  animation: slideInRight 3s forwards;
}

@keyframes slideInRight {
  from {
    transform: translateX(100%);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
} 

.logo img {
  height: 100%;
  width: 100%;
  object-fit: contain;
}
</style>