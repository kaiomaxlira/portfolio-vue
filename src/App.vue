<script lang="ts">

import AboutMe from "./components/AboutMe.vue";
import LogoComponent from "./components/LogoComponent.vue"
import ToolsAndProjects from "./components/ToolsAndProjects.vue";
import Folder from "./components/folder.vue"

export default {
 components: {
   
    AboutMe, 
    LogoComponent,
    ToolsAndProjects,
    Folder,
 }
}
</script>

<template>
   <div class="app">

      <LogoComponent />
      <AboutMe />
      <ToolsAndProjects />
      <Folder />

   </div>
</template>

<style scoped>
.app {
   background-color: #2e3436;
}

</style>