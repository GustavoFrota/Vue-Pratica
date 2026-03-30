<template>
 <div>
  <PrimeiroComponente />
  <p>O dado do epp é {{ testando }}</p>
  <LifeCycle />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'

export default {
  name: "app",
  components: {
    PrimeiroComponente,
    LifeCycle
  },
  data() {
    return {
      testando : "Teste"
    }
  }
}
</script>
