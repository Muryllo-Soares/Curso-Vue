<template>
<div>
  <img  :src="avatar" :alt="descricao"/>
  <MudarImagem @mudar-imagem="trocarImagem" />
</div>

</template>

<script>
import MudarImagem from "./MudarImagem.vue"
export default {
  name: "PicurteFile",
  components:{
    MudarImagem
  },
  data() {
    return {
      avatar: "/img/avatar.png",
      outroavatar: "/img/linkedin.png",
      descricao: "Muryllo Soares",
      
    }
  },
  methods:{
    trocarImagem(){
      this.avatar = this.outroavatar
    }
  }
};
</script>

<style>
img {
  height: 100px;
}
</style>

