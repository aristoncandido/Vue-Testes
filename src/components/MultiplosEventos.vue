<template>
  <div>
    <button @click="primeiro(e), segundo(e)">Ativar Múltiplos Eventos</button>
    <p>{{ multiplos_eventos }}</p>
  </div>
</template>

<script>






export default {
  name: "MultiplosEventos",
  
  data() {
    return {
      multiplos_eventos: "",
    };
  },
  methods: {
    primeiro(e) {
      this.multiplos_eventos = "Primeiro Evento ativado";
    },
    segundo(e) {
      setTimeout(()=>this.multiplos_eventos = 'Segundo Evento', 1000);
    },
  },
};
</script>
