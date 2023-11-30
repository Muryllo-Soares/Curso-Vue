<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event)">Ativar Multiplos Eventos</button>
        <p>{{multiplos_eventos}}</p>
        <ReutilizandoComponents/>
        <ReutilizandoComponents/>
        <ReutilizandoComponents/>
        <ReutilizandoComponents/>
    </div>
</template>

<script>
import ReutilizandoComponents from "./ReutilizandoComponents.vue"
export default {
  name: "MultiplosEventos",
  data(){

    return {
      multiplos_eventos: "",
      txt1 : "Primeiro evento ativado",
      txt2 : "Segundo Evento"
      
   }
  },
  components:{
    ReutilizandoComponents
  },
  methods:{
    primeiro(txt){
      this.multiplos_eventos = txt
    },
     segundo(txt){
    setTimeout(()=> this.multiplos_eventos = txt , 500)
  } 
  },

}
</script>

<style scoped>

</style>