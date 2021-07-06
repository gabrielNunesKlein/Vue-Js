<template>
  <PrimeiroComponente />
  <Lifercycle />
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'; 
import Lifercycle from './components/Lifecycle.vue'; 
  export default {
    name: "App",
    components: {
      PrimeiroComponente,
      Lifercycle
    }
  }
</script>
