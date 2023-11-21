<template>
  <img :src="avatar" :alt="descricao"/>
</template>

<script>
export default {
  name: "PicurteFile",
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Muryllo Soares"
    }
  },
};
</script>

<style>
img {
  height: 100px;
}
</style>

