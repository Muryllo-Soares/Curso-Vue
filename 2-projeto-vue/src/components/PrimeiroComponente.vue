<template>
  <div>
    <h1>Olá Vue</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <p v-if="estou_trabalhando">no momento estou trabalhando</p>
    <p v-else>Não estou trabalhando</p>
    <p v-show="mostrar_email">pode mostrar o meu email: {{ email }}</p>
    <p v-if="2 == 2">Testando</p>
    <Picture />
    <p>
      Segue link para o meu portifolio
      <a v-bind:href="github" target="_blank">GitHub</a>
    </p>
  </div>
</template>

<script>
import Picture from "./Picture.vue";

export default {
  name: "PrimeiroComponente",
  components: {
    Picture,
  },
  data() {
    return {
      nome: "Muryllo",
      profissao: "programador",
      estou_trabalhando: true,
      mostrar_email: false,
      email: "Muryllo428@gmail.com",
      github: "https://github.com/Muryllo-Soares",
    };
  },
};
</script>
