<template>
  <div>
    <p>Estou Trabalhando no momento</p>
    <p>Estou em busca de novas oportunidades!</p>
    <p>Utilizo as seguintes Tecnologias</p>

    <ul>
      <li>JavaScript</li>
      <li>PHP</li>
      <li>Python</li>
    </ul>

    <p v-show="mostrar_email">Mande uma mensagem para {{MeuEmail}}</p>
    <p>
      Para acessar meu portfoliobasta clicar <a v-bind:href="meu_link">aqui</a>
    </p>
    <Emit @mudar-fundo='TrocarFundo'/>
  </div>
</template>

<script>
 import Emit from './emit.vue'
export default {
   
  name: "Info",
  data() {
    return {
      mostrar_email: true,

      meu_link: "https://google.com",
     
 
    };
  },
  props:{
        MeuEmail:String
  },
  components:{
    Emit
  },
  methods:{
   TrocarFundo(){
    document.getElementsByTagName('body')[0].style.backgroundColor = 'black'
   }
  }
};
</script>
