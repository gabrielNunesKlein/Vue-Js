<template>
<div>
  <Header :esta_logado="true"/>
  <PrimeiroComponente />
  <Lifercycle />
  <Pessoa />
</div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import Header from './components/Header.vue'; 
import Lifercycle from './components/Lifecycle.vue'; 
import Pessoa from './components/Pessoa.vue';
  export default {
    name: "App",
    components: {
      Header,
      PrimeiroComponente,
      Lifercycle,
      Pessoa
    }
  }
</script>

<style>
  body{
    background-color: #333;
    color: #fff;
  }
  a{
    color: red;
  }
</style>