<template>
    <div class="container">
        <div class="Content">
            <div class="Foto">
                <img src="../assets/Ali-copia.png" alt="">
            </div>
            <div class="infos">
                <button @click="Seta = !Seta">
                    <img v-if="Seta" src="../assets/seta-para-baixo.png" alt="seta">
                    <img v-else src="../assets/seta-para-cima.png" alt="seta">
                </button>
                <p :class="['text', {'sumir' : Seta}]">Copia da interface inicial do site da Aliexpress feito em react.</p>
            </div>
        </div>

        <div class="Content">
            <div class="Foto">
                <img src="../assets/prev-temp.png" alt="">
            </div>
            <div class="infos">
                <button @click="Seta2 = !Seta2">
                    <img v-if="Seta2" src="../assets/seta-para-baixo.png" alt="seta">
                    <img v-else src="../assets/seta-para-cima.png" alt="seta">
                </button>
                <p :class="['text', {'sumir' : Seta2}]">Site simples de previsão do tempo que pega as informações de uma api externa.</p>
            </div>
        </div>
        
    </div>
    
    
    
</template>


<script>
export default {
    name: 'ProjetoComp',
    data() {
        return {
            Seta: true,
            Seta2: true
        }
    },
}
</script>



<style scoped>
.container {
    width: 90vw;
    margin: auto;
    display: flex;
    gap: 5em;
}

.Foto {
    height: 11em;
    border: 1px solid rgba(128, 128, 128, 0.505);
    width: 22.4em;
}

.Foto:hover {
    height: 12em;
    width: 24.44em;
    transition: 1s;
}

img {
    height: 100%;  
}

.infos {
    display: flex;
    margin-top: 2px;
}

button {
    height: 1em;
    background-color: rgba(128, 128, 128, 0);
    border: none;
}

.text {
    font-size: .8em;
    border-bottom: 1px solid rgba(128, 128, 128, 0.329);
    width: 24.5em;
    padding: 3px;
}
.sumir {
    display: none;
}




</style>