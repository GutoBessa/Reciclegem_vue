<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <mudar-imagem />
  </div>
</template>
<script>
import MudarImagem from '../../../../../Downloads/MudarImagem.vue';
import Reutilizacao from "./Reutilizacao.vue";
export default {
  name: "Pictures",
  components: {
    Reutilizacao,
  },
    MudarImagem
  data() {
    return {
      avatar: "avatar.png",
      descricao: "Luiz Bessa",
    };
  },
};
</script>
