<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>Estou em buscas de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias para back-end.</p>
        <ul>
            <li v-for="(tecnologias, index) in tecnologias_backend" v-bind:key="index">
                {{ tecnologias }}
            </li>
        </ul>
        <p>Utilizo as seguintes tecnologias para front-end.</p>
        <ul>
            <li v-for="tecnologias in tecnologias_frontend" :key="tecnologias.id">
                {{ tecnologias.tecnologia }}
            </li>
        </ul>
        <div>
            <button @click="mostrarEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma menssagem para: {{ email }}</p>
        <p>Acesse meu portifolio <a v-bind:href="meu_portifolio" target="_blank">click aqui</a></p>
        <Perfil />
    </div>
</template>

<script>
import Perfil from './Perfil.vue';
export default{
    name: "Info",
    components: {
        Perfil
    },
    props:{
        email: String
    },
    data(){
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            meu_portifolio: 'https://github.com/gabrielNunesKlein',
            textoBotao: 'Mostrar E-mail',
            tecnologias_backend: ["Python", "Java", "Spring Boot", "Django"],
            tecnologias_frontend: [
                {id: 1, tecnologia: "React Js"},
                {id: 2, tecnologia: "Vue Js"},
                {id: 3, tecnologia: "HML"},
                {id: 4, tecnologia: "CSS"}
            ]
        }
    },
    methods: {
        mostrarEmail(){
            this.mostrar_email = !this.mostrar_email;
            if(!this.mostrar_Email){
                this.textoBotao = 'Mostrar E-mail';
            }else{
                this.textoBotao = 'Esconder E-mail';
            }
        }
    }
}
</script>
