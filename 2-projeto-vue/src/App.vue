/* eslint-disable */
<template>
  <div>
    <Header :esta_logado=true />
    <!-- é possivel passar props das 2 maneiras como objeto determinando o tipo e array não determinando o tipo, e também dados dinamicos via data ou tipados como string boolean etc.. -->
    <PrimeiroComponente :email="email" :estou_trabalhando=true />
    <LifeCycle />
    <FormProject/>
    <br>
    <br>
    <MultiplosEventos/>
  </div>
</template>

<script>
import LifeCycle from "./components/LifeCycle.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import Header from "./components/HeaderProject.vue"
import FormProject from "./components/FormProject.vue"
import MultiplosEventos from "./components/MultiplosEventos.vue"

export default {
  name: "App",
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    FormProject,
    MultiplosEventos,
  },
  data (){
    return {
      email: "Muryllo428@gmail.com"
    }
  }
};
</script>

<style>
  body{
    background-color: lightgray;
    color: black;
  }
  a{
    color: red;
  }
</style>
/* eslint-disable */