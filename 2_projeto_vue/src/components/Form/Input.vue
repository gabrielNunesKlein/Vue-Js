<template>
    <div>
        <h1>Meu Formulario</h1>
        <form @submit="enviarFormulario($event)">
            <div>
                <input type="text" v-model="nome">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <Submit />
            </div>
        </form>
    </div>
</template>

<script>
import Submit from './Submit.vue';
    export default {
        name: 'Input',
        data(){
            return {
                nome: "",
                email: ""
            }
        },
        components: {
            Submit
        },
        methods: {
            enviarFormulario(e){
                e.preventDefault();

                console.log("Formulario enviado")
                const nome = this.nome;
                const email = this.email;
                console.log(`Nome: ${nome}, Email: ${email}`);
            }
        }
    }
</script>