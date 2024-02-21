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
    <div>
      <button @click="show_email">{{ texto_Botao }}</button>
    </div>
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
      mostrar_email: false,
      email: "luiz-augustosouza@hotmail.com",
      texto_Botao: "Mostrar e-mail",
    };
  },
  methods: {
    show_email() {
      this.mostrar_email = !this.mostrar_email;
      if (!this.mostrar_email) {
        this.texto_Botao = "Mostrar email";
      } else {
        this.texto_Botao = "Esconder email";
      }
    },
  },
};
</script>
<style>
.paragrafo-pai {
  color: red;
}
</style>
