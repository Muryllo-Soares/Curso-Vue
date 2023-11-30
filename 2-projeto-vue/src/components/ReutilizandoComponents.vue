<template>
    <div>
        <button @click="ativar()">Cliquei Aqui!</button>
        <span v-show="ativou">Ativado!</span>
    </div>
</template>

<script>
export default {
    name: "ReutilizandoComponents",
    data() {
        return{
            ativou: false
        }
    },

    methods:{
        ativar(){
            this.ativou = !this.ativou
        }
    }
}
</script>