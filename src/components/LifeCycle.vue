<template>
  <h1>{{ loading }}</h1>
</template>

<script>
export default {
  name: "LifeCycle",

  data() {
    return {
      loading: "carregando...",
    };
  },

  created() {
    setTimeout(() => {
      this.loading = "Seja bem vindo";
    }, 3000);
  },

  mounted() {
    setTimeout(() => {
      this.loading = "O que deseja fazer agora?";
    }, 5000);
  },
};
</script>
