<script lang="ts">
import NavBar from "./components/NavBar.vue"
import AboutMe from "./components/AboutMe.vue";
import LogoComponent from "./components/LogoComponent.vue"
import ToolsAndProjects from "./components/ToolsAndProjects.vue";

export default {
 components: {
   NavBar,
    AboutMe, 
    LogoComponent,
    ToolsAndProjects
 }
}
</script>

<template>
   <div class="app">
      <NavBar /> 
      <LogoComponent />
      <AboutMe />
      <ToolsAndProjects />
   </div>
</template>

<style scoped>
.app {
   background-image: linear-gradient( 111.4deg,  rgba(7,7,9,1) 6.5%, rgba(27,24,113,1) 93.2% );
}

</style>