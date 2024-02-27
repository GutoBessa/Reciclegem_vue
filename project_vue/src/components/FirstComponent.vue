<template>
  <div>
    <reutilizacao-vue />
    <h1>Olá Vue!</h1>
    <reutilizacao-vue />
    <p>Meu nome é {{ nome }} e trabalho como {{ Profission }} .</p>
    <multiplos-eventos />
    <reutilizacao-vue />
    <reutilizacao-vue />
    <reutilizacao-vue />
    <reutilizacao-vue />
    <reutilizacao-vue />
    <reutilizacao-vue />
  </div>
</template>
<script>
import ReutilizacaoVue from "./components/Reutilizacao.vue";
import MultiplosEventos from "./MultiplosEventos.vue";

export default {
  name: "FirstComponent",
  components: {
    MultiplosEventos,
    ReutilizacaoVue,
  },
  data() {
    return {
      nome: "Luiz",
      Profission: "Programador",
    };
  },
};
</script>
