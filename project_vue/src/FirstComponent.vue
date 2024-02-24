<template>
  <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ Profission }} .</p>
    <multiplos-eventos />
  </div>
</template>
<script>
import MultiplosEventos from "./MultiplosEventos.vue";
export default {
  name: "FirstComponent",
  components: {
    MultiplosEventos,
  },
  data() {
    return {
      nome: "Luiz",
      Profission: "Programador",
    };
  },
};
</script>
