<template>
    <section>
        <h2>Alguns Projetos</h2>
        <div class="container">
            <Projeto :Foto="Projetos[0].Imagem" :Descricao="Projetos[0].Descri" :Link="Projetos[0].Link" />
            <Projeto :Foto="Projetos[1].Imagem" :Descricao="Projetos[1].Descri" :Link="Projetos[1].Link" />
            <Projeto :Foto="Projetos[2].Imagem" :Descricao="Projetos[2].Descri" :Link="Projetos[2].Link" />
            <Projeto :Foto="Projetos[3].Imagem" :Descricao="Projetos[3].Descri" :Link="Projetos[3].Link" />
            <Projeto :Foto="Projetos[4].Imagem" :Descricao="Projetos[4].Descri" :Link="Projetos[4].Link" />
        </div>
    </section>
</template>


<script>
import Projeto from './ProjetoComp.vue'
import Foto from '../assets/prev-temp.png'
import Foto2 from '../assets/Ali-copia.png'
import Foto3 from '../assets/zap-copia.png'
import Foto4 from '../assets/Compras-htmcss.png'
import Foto5 from '../assets/lista-tarefas.png'

export default {
    name: 'TheProjetos',
    components: {
        Projeto
    },
    data() {
        return {
            Projetos: [{Imagem: Foto, Descri: "Site simples de previsão do tempo que pega as informações de uma api externa.", Link: "https://previsaotemposite.netlify.app/"}, {Imagem: Foto2, Descri: "Copia da interface inicial do site da Aliexpress feito em react.", Link: "https://arthur-zct.github.io/Ali-copia/"}, {Imagem: Foto3, Descri: "Copia da pagina inicial do WhatsApp feita com html e css puro.", Link: "https://arthur-zct.github.io/copia-da-interface-do-whatsapp-web/"}, {Imagem: Foto4, Descri: "Interface inicial de um site de compras feito com html e css.", Link: "https://arthur-zct.github.io/siteV/"}, {Imagem: Foto5, Descri: "Uma simples lista de tarefas.", Link: "https://arthur-zct.github.io/ListadTarefas/"}]
        }
    }
}
</script>



<style scoped>
h2 {
    text-align: center;
    margin-bottom: 1em;
}
.container {
    width: 90vw;
    margin: auto;
    display: flex;
    column-gap: 2vw;
    row-gap: 1.5em;
    flex-wrap: wrap;
    margin-bottom: 5em;
    justify-content: center;
}

@media (max-width: 990px) {
  .container {
    width: 100vw;
    column-gap: 0;
  }
}

</style>