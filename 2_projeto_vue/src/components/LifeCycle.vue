<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    name: "LifeCycle",
    data() {
        return {
            nome: "Ainda não sei"
        }
    },
    created() {
        setTimeout(() => {
        this.nome = "Gustavo"
        }, 1000);

        this.lifecycle()
    },
    mounted() {
        setTimeout(() => {
        this.nome = "Ethan"
        }, 1000);
        this.nome = "Gustavo"
    },
    methods: {
        lifecycle() {
            console.log("Executou")
        }
    }
}

</script>
