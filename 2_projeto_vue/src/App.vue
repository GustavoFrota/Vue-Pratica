<template>
 <div>
  <PrimeiroComponente />
  <p class="paragrafo-pai">O dado do epp é {{ testando }}</p>
  <LifeCycle />
  <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

export default {
  name: "app",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa
  },
  data() {
    return {
      testando : "Teste"
    }
  }
}
</script>

<style>
   body {
    background-color: #333;
    color: #fff;
   }

   a {
    color: red;
   }

   .teste {
    background-color: black;
   }
</style>
