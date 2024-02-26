<template>
  <div>
    <h2>Esta é a descrição da pessoa: {{ name }}</h2>
    <info :email="email" />
    <forms />
  </div>
</template>
<script>
import Forms from "../components/Forms.vue";
import Info from "../components/Info.vue";

export default {
  name: "Person",
  components: {
    Info,
    Forms,
  },
  data() {
    return {
      name: "Luiz",
      email: "luiz-augustosouza@hotmail.com",
    };
  },
};
</script>
