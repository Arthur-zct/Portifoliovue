<template>
  <TheHeader/>
  <main>
    <TheInfos/>
    <div class="linha"></div>
    <TheProjetos/>
  </main>
</template>

<script>
import TheHeader from "./components/TheHeader.vue"
import TheInfos from "./components/TheInfos.vue"
import TheProjetos from "./components/TheProjetos.vue"

export default {
  name: 'App',
  components: {
    TheHeader,
    TheInfos,
    TheProjetos
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background-color: #F4F4F4;
}

.linha {
  height: 1px;
  background-color: rgba(128, 128, 128, 0.349);
  width: 90vw;
  margin: auto;
  margin-top: 20px;
  margin-bottom: 20px;
}

@media (max-width: 1450px) {
  main {
    font-size: 15px;
  }
}

@media (max-width: 1390px) {
  main {
    font-size: 14px;
  }
}

@media (max-width: 912px) {
  main {
    font-size: 25px;
  }
}

@media (max-width: 759px) {
  main {
    font-size: 14px;
  }
}

@media (max-width: 300px) {
  main {
    font-size: 13px;
  }
}

</style>
