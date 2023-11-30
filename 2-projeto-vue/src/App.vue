/* eslint-disable */
<template>
  <div>
    <Header/>
    <PrimeiroComponente />
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