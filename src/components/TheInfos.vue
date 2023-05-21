<template>
    <section>
        <section class="sobre">
            
            <div class="button">
                <h2>
                    Sobre 
                    <button @click="Seta = !Seta">
                        <img v-if="Seta" src="../assets/seta-para-baixo.png" alt="seta">
                        <img v-else src="../assets/seta-para-cima.png" alt="seta">
                    </button>
                </h2>
            </div>
            <div :class="['sobretext', {'sumir' : Seta}]">
                <p>
                    No ano de 2021 eu conheci a programação pela primeira vez e logo me interessei por ela, parecia dificil mas interessante. Eu pesquisei e estudei um pouco mas a escola e o enem estavam ocupando muito do meu tempo e eu acabei deixando de lado, com o fim daquele ano e o começo de um novo eu voltei a ver coisas sobre programação e decidi que queria seguir este caminho, com isso eu ingressei em uma faculdade de Análise e desenvolvimento de sistemas e iniciei meus estudos na area com foco nas tecnologias para o front-end. <br/> Eu sou um cara bem caseiro, gosto de filmes, séries, desenhos, mangás e jogos.
                </p>  
            </div>
            
            
        </section>
    </section>
</template>

<script>
export default {
    name: 'TheInfos',
    data() {
        return {
            Seta: true
        }
    },
}
</script>

<style scoped>
.sobre {
    align-content: center;
}

.sobretext {
    width: 50vw;
    padding: .7em;
    padding-left: .8em;
    border: 1px solid rgba(128, 128, 128, 0.152);
    border-radius: 1em;
    text-align: left;
    text-indent: 3px;
    margin: auto;
    margin-top: 3px;
}

.button {
    text-align: center;
}

.button h2 {
    height: 1.5em;
}

.button button {
    height: 45%;
    margin-top: 1,1em;
    border: none;
    background-color: rgba(255, 255, 255, 0);
    cursor: pointer;
}

img {
    height: 100%;
}

.sumir {
    display: none;
}

</style>