<template>
  <header>
    <h1>Arthur Ivano</h1>
    <div class="infos">
      <p>20 anos - Desenvolvedor web</p>
    </div>
    
    <div class="Links">
      <a href="https://github.com/Arthur-zct">
        <img src="../assets/github.png" alt="github icon">
      </a>
      <a href="https://www.linkedin.com/in/arthur-da-cunha-aa2219256/">
        <img src="../assets/linkedin.png" alt="linkedin icon">
      </a>
    </div>
  </header>
</template>

<script>
export default {
  name: 'TheHeader',
  props: {}
}
</script>

<style scoped>
header {
  margin-bottom: 2em;
  margin-top: 1.1em;
}

h1 {
  width: 250px;
  margin: auto;
  padding-left: 12px;
  font-size: 2.5em;
}

div {
  width: 220px;
  margin: auto;
  margin-top: .5em;
}

.Links {
  height: 30px;
  width: 8em;
}
.Links > a {
  height: 100%;
  margin-left: 1em;
}
.Links > a > img {
  height: 100%;
}

@media (max-width: 1300px) {
  .infos {
    font-size: 1.5em;
    width: 14em;
  }
}

@media (max-width: 280px) {
  .infos {
    font-size: 1em;
    width: 14em;
  }
}

</style>
