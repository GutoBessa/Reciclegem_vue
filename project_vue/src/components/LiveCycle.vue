<template>
  <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
  name: "LiveCycle",
  data() {
    return {
      nome: "I dont know ",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Matheus";
    }, 1111);

    this.lifecycle();
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Pedro";
    }, 2111);
  },
  methods: {
    lifecycle() {
      console.log("Executou!");
    },
  },
};
</script>
