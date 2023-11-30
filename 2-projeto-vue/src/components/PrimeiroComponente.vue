<template>
  <div>
    <p>{{email}}</p>
    <h1>Olá Vue</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>

    <p v-if="estou_trabalhando">no momento estou trabalhando</p>

    <p v-else>Não estou trabalhando</p>

    <p>Utilizo as seguintes tecnologias para back-end:</p>

    <ul>
      <li 
      v-for="(tecnology, index) in backend_technologies" v-bind:key="index">
        {{tecnology}}
      </li>
    </ul>

    <p>Utilizo as seguintes tecnologias para fron-end:</p>

    <ul>
      <li 
      v-for="(tecnology) in frontend_technologies" :key="tecnology.id">
       {{tecnology.language}} 
      </li>
    </ul>

    <button @click="showEmail">{{textoBotao}}</button>

    <p v-show="mostrar_email">pode mostrar o meu email: {{ email }}
    </p>

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
  props:{
        email: String,
        estou_trabalhando: Boolean,
      },
  data() {
    return {
      nome: "Muryllo",
      profissao: "programador",
      
      mostrar_email: false,
      
      github: "https://github.com/Muryllo-Soares",
      textoBotao: "Mostrar email",
      backend_technologies: ['Javascript', 'PHP', 'Python'],
      frontend_technologies: [
        {id: 1, language:"HTML",},
        {id: 2, language:"CSS"},
        {id: 3, language:"VUE"},
        
      ],
    };
  },
  methods:{
    showEmail(){
      this.mostrar_email = !this.mostrar_email
      if(!this.mostrar_email) {
        this.textoBotao = "Mostrar email"
      } else{
        this.textoBotao = "Esconder email"
      }
    }
  }
};
</script>
