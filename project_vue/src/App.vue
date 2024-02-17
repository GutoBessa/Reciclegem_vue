<template>
  <div>
    <first-component-vue />
    <p>O dado de app é {{ Testando }} .</p>
    <live-cycle-vue />
    <person />
  </div>
</template>
<script>
import LiveCycleVue from "./components/LiveCycle.vue";
import Person from "./components/Person.vue";
import FirstComponentVue from "./FirstComponent.vue";

export default {
  name: "App",
  components: {
    FirstComponentVue,
    LiveCycleVue,
    Person,
  },
  data() {
    return {
      Testando: "Teste",
    };
  },
};
</script>
