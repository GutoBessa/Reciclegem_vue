<template>
  <div>
    <h2>Meu Formulário:</h2>
    <form action="">
      <div>
        <input-teext-vue />
      </div>
      <div>
        <input-teext-vue />
      </div>
      <div>
        <submitt-vue />
      </div>
    </form>
  </div>
</template>
<script>
import InputTeextVue from "./InputTeext.vue";
import SubmittVue from "./Submitt.vue";
export default {
  name: "Forms",
  components: {
    InputTeextVue,
    SubmittVue,
  },
};
</script>
