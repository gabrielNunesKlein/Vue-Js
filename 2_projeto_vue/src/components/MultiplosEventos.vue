<template>
    <div>
        <button @click="primeiro(txt1), segundo(txt2), terceiro()">Ativar Eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
    export default{
        name: 'MultiplosEventos',
        data(){
            return{
                multiplos_eventos: "",
                txt1: "Primeiro evento !",
                txt2: "Segundo Evento !"
            }
        },
        methods:{
            primeiro(txt){
                this.multiplos_eventos = txt;
            },
            segundo(txt){
                setTimeout(() => this.multiplos_eventos = txt, 500)
            },
            terceiro(){
                setTimeout(() => this.multiplos_eventos = "", 1500)   
            }
        }
    }
</script>


<style scoped>
    div{
        padding: 100px;
    }
</style>
