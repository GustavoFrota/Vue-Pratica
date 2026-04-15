<template>
  <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e eu sou um {{ ocupação }}</p>
    <MultiplosEventos />
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'

 export default {
    name: "PrimeiroComponente",
    components: {
      MultiplosEventos

    },
    data() {
        return {
            nome: "Gustavo",
            ocupação: "estudante"
        }
    }
 }
</script>