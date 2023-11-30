<template>
  <div class="header">
    <ul>
      <li>HOME</li>
      <li>BLOG</li>
      <li>CONTANTO</li>
      <li v-if="esta_logado"> <a href="#">Meu Perfil</a></li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "HeaderProject",
  props:["esta_logado"],
  data() {},
};
</script>

<style scoped>
.header > ul {
  display: flex;
  flex-direction: row;
  gap: 15px;
  list-style: none;
}
</style>
