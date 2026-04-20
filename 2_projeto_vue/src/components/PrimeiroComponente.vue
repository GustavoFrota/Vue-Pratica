<template>
  <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e eu sou um {{ ocupação }}</p>
    <MultiplosEventos />
    <Reutilizacao />
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizacao from './Reutiizacao.vue'

 export default {
    name: "PrimeiroComponente",
    components: {
      MultiplosEventos,
      Reutilizacao

    },
    data() {
        return {
            nome: "Gustavo",
            ocupação: "estudante"
        }
    }
 }
</script>