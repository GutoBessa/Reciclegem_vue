<template>
  <div>
    <p v-if="Esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oprtunidades.</p>
    <p>Utilizo as sequintes tecnologias:</p>
    <ul>
      <li
        v-for="(technology, index) in backend_technologies"
        v-bind:key="index"
      >
        {{ technology }}
      </li>
    </ul>
    <p>Utilizo as sequintes technologias para front-end:</p>
    <ul>
      <li v-for="technology in frontend_technologies" :key="technology.id">
        {{ technology.language }}
      </li>
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
  name: "Infoo",
  components: {
    Pictures,
  },
  props: {
    email: String,
  },
  data() {
    return {
      Esta_trabalhando: false,
      mostrar_email: false,
      texto_Botao: "Mostrar e-mail",
      backend_technologies: ["Javascript", "PHP", "Python"],
      frontend_technologies: [
        { id: 1, language: "HTML" },
        { id: 2, language: "CSS" },
        { id: 3, language: "VUE" },
      ],
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
