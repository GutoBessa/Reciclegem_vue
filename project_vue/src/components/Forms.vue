<template>
  <div>
    <h2>Meu Formulário:</h2>
    <form action="" @submit="enviarFormulario($event)">
      <div>
        <input type="text" v-model="name" />
      </div>
      <div>
        <input type="text" v-model="email" />
      </div>
      <div>
        <submitt-vue />
      </div>
    </form>
    <p>Conteudo</p>
    <p>Conteudo</p>
    <p>Conteudo</p>
  </div>
</template>
<script>
import InputTeextVue from "./InputTeext.vue";
import SubmittVue from "./Submitt.vue";
export default {
  name: "Forms",
  components: {
    InputTeextVue,
    SubmittVue,
  },
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Formulário Enviado!");
      console.log("o nome é: " + name);
      console.log("o email é: " + email);
    },
  },
};
</script>
<style scoped>
p {
  margin: 151px;
}
</style>
