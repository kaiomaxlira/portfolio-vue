<script lang="ts">
import NavBar from "../components/NavBar.vue"

export default {
  components: {
    NavBar,
  },
  data() {
    return {
      spanVisible: true, // Inicialmente visível
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
    this.handleScroll(); // Chama a função handleScroll inicialmente
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      const scrollPosition = window.scrollY || window.scrollY;
      const scrollThreshold = 300; // Posição de rolagem para ocultar o nome "KAIO"
      // Verifica se a posição de rolagem ultrapassou o limite definido
      this.spanVisible = scrollPosition < scrollThreshold;
    },
  },
};
</script>

<template>
  <body>
    <div class="background">
      <NavBar /> 
      <div class="logo" ref="container">
        <span :class="{ kaio: spanVisible, 'animation-left': !spanVisible }"
          >KAIO</span
        >
        <img
          :class="{ 'logo-img': spanVisible, 'logo-img-out': !spanVisible }"
          src="../assets/img/3angulo.ico"
          alt="logo"
        />
        <span :class="{ max: spanVisible, 'animation-right': !spanVisible }"
          >MAX</span
        >
      </div>
    </div>
  </body>
</template>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 615px;
  width: 100%;
  overflow: hidden;
}

.background {
  background-image: url('../assets/img/cidade2.jpg');
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 100%;

}

.logo {
  margin-top: 8rem;
  height: 210px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.logo img {
  height: 90%;
  width: 90%;
  object-fit: contain;
}

.logo-img {
  opacity: 0;
  animation: zoomIn 4s forwards;
}

.logo-img-out {
  opacity: 0;
  animation: zoomOut 4s forwards;
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
@keyframes zoomOut {
  from {
    transform: scale(1);
    opacity: 1;
  }
  to {
    transform: scale(0);
    opacity: 0;
  }
}

.kaio {
  color: #989c90;
    font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  opacity: 0;
  animation: slideInLeft 3s forwards;
}

@keyframes slideInLeft {
  from {
    transform: translateX(-450px);
    opacity: 0;
  }
  to {
    transform: translateX(35%);
    opacity: 1;
  }
}

@keyframes slideKaioOut {
  from {
    transform: translateX(35%);
    opacity: 1;
  }
  to {
    transform: translateX(-450px);
    opacity: 0;
  }
}

.animation-left {
  color: #989c90;
  transition: opacity 0.5s ease;
  opacity: 0;
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  animation: slideKaioOut 4s forwards;
}

.max {
  color: #989c90;
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
    transform: translateX(450px);
    opacity: 0;
  }
  to {
    transform: translateX(-40%);
    opacity: 1;
  }
}
@keyframes slideMaxOut {
  from {
    transform: translateX(-40%);
    opacity: 1;
  }
  to {
    transform: translateX(450px);
    opacity: 0;
  }
}

.animation-right {
  color: #989c90;
  transition: opacity 0.5s ease-out;
  opacity: 0;
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  margin-left: 12px;
  animation: slideMaxOut 4s forwards;
}
</style>