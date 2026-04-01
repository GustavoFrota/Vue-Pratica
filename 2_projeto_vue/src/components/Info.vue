<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizando as seguintes tecnologias:</p>
    <ul>
        <li>JavaScript</li>
        <li>PHP</li>
        <li>Python</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p>Para acessar meu portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    </div>
</template>

<script>
export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: true,
            email: "gustavo@gmail.com",
            meu_link: "https://google.com"
        }
    }
   
}
</script>