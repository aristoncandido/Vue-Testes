<template>
    <div>
        <h2>Está é aminha pessoa:</h2>
        <Info MeuEmail='exemplo@gmail.com'/>
        <Info MeuEmail='oxiii'/>
        <Form/>

    </div>
</template>


<script>
import Info from './Info.vue'
import Form from './Form.vue'

export default {
    name:'Pessoa',
    data(){
        return{
            nome:'Ariston'
        }
    },
    components:{
        Info,
        Form
      }  
}
</script>