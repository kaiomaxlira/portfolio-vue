<script lang="ts">

import AboutMe from "./components/AboutMe.vue";
import LogoComponent from "./components/LogoComponent.vue"
import ToolsAndProjects from "./components/ToolsAndProjects.vue";

export default {
 components: {
   
    AboutMe, 
    LogoComponent,
    ToolsAndProjects
 }
}
</script>

<template>
   <div class="app">

      <LogoComponent />
      <AboutMe />
      <ToolsAndProjects />
   </div>
</template>

<style scoped>
.app {
   background-color: #2e3436;
}

</style>