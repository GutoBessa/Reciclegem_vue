<template>
  <img :src="avatar" :alt="descricao" />
</template>
<script>
export default {
  name: "Pictures",
  data() {
    return {
      avatar: "avatar.png",
      descricao: "Luiz Bessa",
    };
  },
};
</script>
