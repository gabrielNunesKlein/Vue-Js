<template>
<div>
    <h1>Está descrição da pessoa: {{ name }}</h1>
    <Info :email="email"/>
    <Form />
</div>
</template>

<script>
import Info from './Info.vue';
import Form from './Form/Input.vue';
export default {
    name: "Pessoa",
    components:{
        Info,
        Form
    },
    data(){
        return{
            name: "Gabriel",
            email: "Gabriel@gmail.com"
        }
    }
}
</script>
