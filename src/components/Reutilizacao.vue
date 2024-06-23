<template>
    <div>
        <button @click="ativar">Clique aqui</button>
        <p v-show="ativou">Ativado</p>
    </div>
</template>

<script>
export default{
    name:'Reutilizacao',
    data(){
        return{
            ativou:false
        };
    },

    methods:{
        ativar(){
            this.ativou = !this.ativou;
        }
    }
}
</script>
<style scoped>
div{
    display: flex;
}
</style>