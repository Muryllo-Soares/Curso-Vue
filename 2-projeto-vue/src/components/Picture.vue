<template>
<div>
  <button @click="showImagem">Mudar imagem</button>
  <img  :src="avatar" :alt="descricao"/>
</div>

</template>

<script>
export default {
  name: "PicurteFile",
  data() {
    return {
      avatar: "/img/avatar.png",
      outroavatar: "/img/linkedin.png",
      descricao: "Muryllo Soares",
      
    }
  },
  methods:{
    showImagem(){
        if(this.avatar == this.avatar){
          this.avatar = this.outroavatar
        } else(
          this.avatar = "/img/avatar.png"
        )
        
    }
  }
};
</script>

<style>
img {
  height: 100px;
}
</style>

