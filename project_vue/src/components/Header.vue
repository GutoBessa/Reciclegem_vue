<template>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Projeto</a></li>
    <li><a href="#">Contato</a></li>
    <li v-if="esta_logado"><a href="#">Meu perfil</a></li>
  </ul>
</template>
<script>
export default {
  name: "Header",
  props: ["esta_logado"],
};
</script>

<style scoped>
ul {
  list-style: none;
  display: flex;
  background-color: #999;
}

li {
  margin-right: 11px;
}

a {
  color: #ddd;
  text-decoration: none;
  transition: 0.5s;
}

a:hover {
  color: transparent;
}
</style>
