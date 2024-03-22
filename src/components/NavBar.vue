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
      target.style.color = "#808080";
    },
    resetEffect(event: MouseEvent) {
      const target = event.target as HTMLElement;
      target.style.transition = "color 0.5s";
      target.style.color = "#000";
      
    }
  }
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: center;
  padding-top: 3rem;
}

.nav a {
  color: #000;
  text-align: center;
  padding-top: 10rem;
  text-decoration: none;
  font-size: 23px;
  margin: 57px;
}
</style>
