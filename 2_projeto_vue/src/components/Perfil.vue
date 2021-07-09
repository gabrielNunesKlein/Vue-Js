<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <Reutilizacao />
    </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue';
    export default {
        name: "Perfil",
        components: {
            Reutilizacao
        },
        data(){
            return {
                avatar: '/img/avatar-blank.png',
                descricao: 'Gabriel Klein'
            }
        }
    }
</script>
