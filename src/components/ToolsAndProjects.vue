<script lang="ts">
export default {
  name: "ToolsAndProjects",
  components: {},
};
</script>

<template>
  <div class="ToolsAndProjects">
      <div class="container_project"></div>
      <div class="container_tool"></div>
      
  </div>
</template>

<style scoped>
.ToolsAndProjects {
  margin: 0;
  width: 100%;
  height: 615px;
  display: flex;
  gap: 15rem;
  align-items: center;
  justify-content: center;
}

.container_project,
.container_tool {
  width: 30rem;
  height: 35rem;
  border-radius: 10% 10% 10% 10%;
  border-right: 0px solid black;
  border-bottom: 0px solid black;
  border-top: 0px solid black;
  border-left: 0px solid black;
  box-shadow: 0 0 10px #6391FF;
}

</style>