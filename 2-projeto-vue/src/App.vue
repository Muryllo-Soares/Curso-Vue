/* eslint-disable */
<template>
  <div>
    <Header/>
    <PrimeiroComponente />
    <LifeCycle />
  </div>
</template>

<script>
import LifeCycle from "./components/LifeCycle.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import Header from "./components/HeaderProject.vue"

export default {
  name: "App",
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
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