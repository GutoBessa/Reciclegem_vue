<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <reutilizacao />
  </div>
</template>
<script>
import Reutilizacao from "./Reutilizacao.vue";
export default {
  name: "Pictures",
  components: {
    Reutilizacao,
  },
  data() {
    return {
      avatar: "avatar.png",
      descricao: "Luiz Bessa",
    };
  },
};
</script>
