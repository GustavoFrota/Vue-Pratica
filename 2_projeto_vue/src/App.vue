<template>
 <div>
  <PrimeiroComponente />
  <p>O dado do epp é {{ testando }}</p>
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'

export default {
  name: "app",
  components: {
    PrimeiroComponente
  },
  data() {
    return {
      testando : "Teste"
    }
  }
}
</script>
