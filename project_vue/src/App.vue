<template>
  <div>
    <first-component-vue />
    <p>O dado de app é {{ Testando }} .</p>
    <live-cycle-vue />
  </div>
</template>
<script>
import LiveCycleVue from "./components/LiveCycle.vue";
import FirstComponentVue from "./FirstComponent.vue";

export default {
  name: "App",
  components: {
    FirstComponentVue,
    LiveCycleVue,
  },
  data() {
    return {
      Testando: "Teste",
    };
  },
};
</script>
