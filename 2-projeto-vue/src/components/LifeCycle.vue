/* mostrando algumas funcionalidades do lyfecycle do vue */


<template>
    <h1>Meu nome é: {{nome}}</h1>
</template>

<script>
export default {
    name:"LifeCycleHooks",
    data(){
        return{
            nome: "Ainda não sei",
        }
    },
    created(){
        setTimeout(()=>{
            this.nome = "Muryllo"
        }, 1000)
        this.lifeCycle()
    },
    mounted(){
        setTimeout(()=>{
            this.nome = "Amanda"
        }, 2000)
        this.lifeCycle()
    },

    methods:{
        lifeCycle(){
            console.log("executou")
        }
    }


}
</script>