<template>
<div>
  <PrimeiroComponente />
  <Lifercycle />
  <Pessoa />
</div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'; 
import Lifercycle from './components/Lifecycle.vue'; 
import Pessoa from './components/Pessoa.vue';
  export default {
    name: "App",
    components: {
      PrimeiroComponente,
      Lifercycle,
      Pessoa
    }
  }
</script>
