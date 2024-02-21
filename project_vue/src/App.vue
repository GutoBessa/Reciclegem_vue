<template>
  <div>
    <Header />
    <first-component-vue />
    <p class="paragrafo-pai">O dado de app é {{ Testando }} .</p>
    <live-cycle-vue />
    <person />
  </div>
</template>
<script>
import LiveCycleVue from "./components/LiveCycle.vue";
import Person from "./components/Person.vue";
import FirstComponentVue from "./FirstComponent.vue";
import Header from "./Header.vue";

export default {
  name: "App",
  components: {
    FirstComponentVue,
    LiveCycleVue,
    Person,
    Header,
  },
  data() {
    return {
      Testando: "Teste",
    };
  },
};
</script>
<style>
body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}

.teste {
  background-color: #000;
}
</style>
