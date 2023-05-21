<template>
    <section>
        <h2>Projetos</h2>
        <div>
            <Projeto />
        </div>
        
    </section>
</template>


<script>
import Projeto from './ProjetoComp.vue'

export default {
    name: 'TheProjetos',
    components: {
        Projeto
    },
}
</script>



<style scoped>
h2 {
    text-align: center;
    margin-bottom: 1em;
}

div {
    gap: 5em;
}
</style>