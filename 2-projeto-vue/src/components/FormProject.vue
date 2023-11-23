<template>
<div>
    <h2>Meu formulário:</h2>
    <form @submit="enviarFormulario($event)">
        <div>
            <input type="text" v-model="nome">
        </div>
        <div>
            <input type="email" v-model="email">
        </div>
        <button type="submit">Enviar</button>
    </form>
</div>
</template>

<script>
export default {
    name: "FormProject",

    data(){
        return{
            nome: "",
            email: ""
        }
    },

    methods:{
        enviarFormulario(e){

        e.preventDefault();

        const nome = this.nome
        const email = this.email
           
        console.log(`Meu nome é: ${nome}`)
        console.log(`Meu email é: ${email}`)

        // Inserir no banco de dados
        }
    }
}
</script>