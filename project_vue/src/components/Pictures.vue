<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <MudarImagem @mudar-imagem="TrocarImagem" />
  </div>
</template>
<script>
import MudarImagem from "../components/MudarImagem.vue";

export default {
  name: "Pictures",
  components: {
    MudarImagem,
  },

  data() {
    return {
      avatar: "../img/avatar.png",
      descricao: "Luiz Bessa",
    };
  },
  methods: {
    TrocarImagem() {
      this.avatar = "../img/avatar2.png";
    },
  },
};
</script>
