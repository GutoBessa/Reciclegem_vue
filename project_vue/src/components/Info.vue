<template>
  <div>
    <p v-if="Esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oprtunidades.</p>
    <p>Utilizo as sequintes tecnologias:</p>
    <ul>
      <li>JavaScript</li>
      <li>PHP</li>
      <li>Python</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p>
      Para acessar meu portifólio
      <a v-bind:href="meu_link" target="_blank">Basta clicar</a>
    </p>
    <Pictures />
  </div>
</template>
<script>
import Pictures from "./Pictures.vue";
export default {
  components: { Pictures },
  name: "Infoo",
  data() {
    return {
      Esta_trabalhando: false,
      mostrar_email: true,
      email: "luiz-augustosouza@hotmail.com",
    };
  },
};
</script>
