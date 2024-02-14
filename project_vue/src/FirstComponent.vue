<template>
  <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ Profission }} .</p>
  </div>
</template>
<script>
export default {
  name: "FirstComponent",
  data() {
    return {
      nome: "Luiz",
      Profission: "Programador",
    };
  },
};
</script>
