<script lang="ts">
export default {
  components: {},
};
</script>

<template>
  <body>
    <div class="logo">
      <span data-aos="fade-right" data-aos-duration="1000" class="kaio">KAIO</span>
      <img data-aos="zoom-out" data-aos-duration="1000" src="../assets/img/kaio.png" alt="logo" />
      <span data-aos="fade-left" data-aos-duration="1000" class="max">MAX</span>
    </div>
  </body>
</template>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 9rem;
  width: 0rem;
  margin: 0;
}

.logo {
  height: 210px;
  width: 200px;
  margin-left: 33rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.kaio {
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
}
.max {
  font-size: 150px;
  font-family: "Archivo Black", sans-serif;
  font-weight: 900;
  font-style: normal;
  margin-left: 12px;
}

.logo img {
  height: 100%;
  width: 100%;
  object-fit: contain;
}
</style>
