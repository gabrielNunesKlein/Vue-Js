<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default {
        name: "Perfil",
        data(){
            return {
                avatar: '/img/avatar-blank.png',
                descricao: 'Gabriel Klein'
            }
        }
    }
</script>
