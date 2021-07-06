<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>Estou em buscas de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias.</p>
        <ul>
            <li>Python</li>
            <li>Java</li>
            <li>JavaScript</li>
        </ul>
        <p v-show="mostrar_email">Mande uma menssagem para: {{ email }}</p>
    </div>
</template>

<script>
export default{
    name: "Info",
    data(){
        return {
            esta_trabalhando: false,
            mostrar_email: true,
            email: 'Gabriel.klein@gmail.com'
        }
    }
}
</script>
