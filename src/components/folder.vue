<script lang="ts">
export default {
  name: "FolderAndExperience",
  components: {},
};
</script>

<template>
  <div class="Folder">
    <span class="ExperienceAndEducation">Experiências & Educação</span>

    <div class="opcoes">
      <div class="Experiencias">
        <button>Compass</button>
      </div>

      <div class="Educacao">
        <button>Compass</button>
      </div>

    </div>
  </div>
</template>

<style scoped>
.Folder {
  margin: 0;
  margin-top: 2rem;
  width: 100%;
  height: 615px;
  text-align: center;
}

.ExperienceAndEducation {
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
  font-size: 2.5rem;
  color: #989c90;
}

.opcoes {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10rem;

}

/* Experiencias */

.Experiencias {
  border-width: 5px;
  border-style: solid;
  border-color: aqua;
  height: 25rem;
  width: 30rem;
}

/* Educacao */

.Educacao {
  border-width: 5px;
  border-style: solid;
  border-color: aqua;
  height: 25rem;
  width: 30rem;
}

button {
  font-size: 18px;
  color: #e1e1e1;
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  cursor: pointer;
  position: relative;
  border: none;
  background: none;
  text-transform: uppercase;
  transition-timing-function: cubic-bezier(0.25, 0.8, 0.25, 1);
  transition-duration: 400ms;
  transition-property: color;
}

button:focus,
button:hover {
  color: #fff;
}

button:focus:after,
button:hover:after {
  width: 100%;
  left: 0%;
}

button:after {
  content: "";
  pointer-events: none;
  bottom: -2px;
  left: 50%;
  position: absolute;
  width: 0%;
  height: 2px;
  background-color: #fff;
  transition-timing-function: cubic-bezier(0.25, 0.8, 0.25, 1);
  transition-duration: 400ms;
  transition-property: width, left;
}
</style>
