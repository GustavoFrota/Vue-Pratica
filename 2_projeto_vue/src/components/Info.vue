<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizando as seguintes tecnologias para back-end:</p>
    <ul v-for="technology, index in backend_tecnologies" v-bind:key="index">
        <li> {{ technology }}</li>
    </ul>
    <div>
        <button @click="showEmail"> {{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p class="teste">Para acessar meu portfólio <a :href="meu_link" target="_blank">basta clicar aqui</a></p>
    </div>
</template>

<script>
export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "gustavo@gmail.com",
            meu_link: "https://google.com",
            textoBotao: "Mostrar e-mail",
            backend_tecnologies: ['Javascript', 'PHP', "Python"]
        }
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email) {
                this.textoBotao = "Mostrar e-mail"
            } else {
                this.textoBotao = "Esconder e-mail"
            }
        }
    }
   
}
</script>

<style>
  .paragrafo-pai {
    color: red;
  }
</style>