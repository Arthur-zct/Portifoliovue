<template>
    <div class="content_container">
        <div class="Content">
            
            <div class="Foto">
                <a :href="Link">
                    <img :src="Foto" alt="">
                </a>
            </div>
            <div class="infos">
                <button @click="Seta = !Seta">
                    <img v-if="Seta" src="../assets/seta-para-baixo.png" alt="seta">
                    <img v-else src="../assets/seta-para-cima.png" alt="seta">
                </button>
                <p :class="['text', {'sumir' : Seta}]">{{ Descricao }}</p>
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
        }
    },
    props: {
        Foto: String,
        Descricao: String,
        Link: String
    }
}
</script>



<style scoped>
* {
    margin: 0;
}
.content_container {
    height: 13em;
    width: 26em;
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
    width: 100%; 
}

.infos {
    display: flex;
    margin-top: 2px;
}

button {
    height: 1.5em;
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

@media (max-width: 1300px) {
    .Foto:hover {
        height: 11em;
        width: 24.32em;
    }

    .Foto {
        height: 11em;
        border: 1px solid rgba(128, 128, 128, 0.505);
        width: 22.32em;
    }

    .text {
    font-size: .9em;
    border-bottom: 1px solid rgba(128, 128, 128, 0.329);
    width: 22em;
    padding: 3px;
}
}

@media (max-width: 990px) {
  .content_container {
    width: 24em;
  }
}

@media (max-width: 900px) {
    .Foto {
        height: 10em;
        border: 1px solid rgba(128, 128, 128, 0.505);
        width: 20.32em;
    }

    .content_container {
        width: 20.6em;
    }
}

@media (max-width: 280px) {
    .Foto {
        height: 10em;
        border: 1px solid rgba(128, 128, 128, 0.505);
        width: 20em;
    }

    .content_container {
        width: 20.6em;
    }
}

</style>