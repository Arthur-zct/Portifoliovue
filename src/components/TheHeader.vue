<template>
  <header>
    <h1>Arthur Ivano</h1>
    <div class="infos">
      <p>19 anos - Desenvolvedor web</p>
    </div>
    
    <div class="Links">
      <a href="">
        <img src="../assets/github.png" alt="">
      </a>
      <a href="">
        <img src="../assets/linkedin.png" alt="">
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
  margin-bottom: 1em;
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
  text-align: center;
}
.Links > a {
  height: 100%;
  margin-left: 10px;
}
.Links > a > img {
  height: 100%;
}

</style>
