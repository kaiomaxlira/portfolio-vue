<template>
  <header>
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="nav">
        <a href="#home" @mouseover="hoverEffect($event)" @mouseleave="resetEffect">Home</a>
        <a href="#news" @mouseover="hoverEffect($event)" @mouseleave="resetEffect">News</a>
        <a href="#contact" @mouseover="hoverEffect($event)" @mouseleave="resetEffect">Contact</a>
      </div>
    </nav>
  </header>
</template>

<script lang="ts">
export default {
  methods: {
    hoverEffect(event: MouseEvent) {
      const target = event.target as HTMLElement;
      target.style.transition = "color 0.5s"; 
      target.style.color = "#bc6c64";
    },
    resetEffect(event: MouseEvent) {
      const target = event.target as HTMLElement;
      target.style.transition = "color 0.5s";
      target.style.color = "#989c90";
      
    }
  }
}
</script>

<style scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 60px;
  background-color: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(5px);
}

.nav a {
  color: #989c90;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-style: italic;
  text-align: center;
  padding-top: 10rem;
  text-decoration: none;
  font-size: 1.3rem;
  margin: 57px;
}
</style>
