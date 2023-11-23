<template>
  <div class="header">
    <ul>
      <li>HOME</li>
      <li>BLOG</li>
      <li>CONTANTO</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "HeaderProject",
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
