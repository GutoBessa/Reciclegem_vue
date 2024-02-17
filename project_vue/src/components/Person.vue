<template>
  <div>
    <h2>Esta é a descrição da pessoa: {{ name }}</h2>
    <info />
    <forms />
  </div>
</template>
<script>
import Forms from "../components/Forms.vue";
import Info from "../components/Info.vue";
export default {
  components: { Info, Forms },

  Formname: "Person",
  data() {
    return {
      name: "Luiz",
    };
  },
};
</script>
