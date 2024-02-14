<template>
  <div>
    <first-component-vue />
    <p>O dado de app é {{ Testando }} .</p>
  </div>
</template>
<script>
import FirstComponentVue from "./FirstComponent.vue";

export default {
  name: "App",
  components: {
    FirstComponentVue,
  },
  data() {
    return {
      Testando: "Teste",
    };
  },
};
</script>
