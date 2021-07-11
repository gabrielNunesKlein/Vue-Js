<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <TrocaImagem @mudar-Imagem="trocarImagem"/>
    </div>
</template>

<script>
import TrocaImagem from './TrocaImagem.vue';
    export default {
        name: "Perfil",
        components: {
            TrocaImagem
        },
        data(){
            return {
                avatar: 'img/avatar-blank.png',
                descricao: 'Gabriel Klein'
            }
        },
        methods:{
            trocarImagem(){
                this.avatar = 'img/avatar2.png'
            }
        }
    }
</script>
