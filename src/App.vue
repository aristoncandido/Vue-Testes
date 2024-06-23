<template>
  <div>
    <PrimeiroComponente />
    <h2>Usando LifeCycle</h2>
    <HR></HR>
    <LifeCycle />
    <Form v-show="aparecer"/>
    <Info/>
    <Reutilizacao/>

    <Reutilizacao/>

    <Reutilizacao/>

    <Reutilizacao/>

    <Reutilizacao/>
    <Pessoa/>
  </div>
</template>

<script>
import LifeCycle from "./components/LifeCycle.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import Form from "./components/Form.vue"
import Info from "./components/Info.vue"
import Reutilizacao from './components/Reutilizacao.vue';
import Pessoa from './components/Pessoa.vue'
export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Form,
    Info,
    Reutilizacao,
    Pessoa
  },
  data() {
    return {
      nome: "Ariston",
      trabalho: "Fodisse",
      aparecer:true
    };
  },
};
</script>
