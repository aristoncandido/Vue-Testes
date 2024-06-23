<template>
    <div>
        <button @click="$emit('mudarFundo')" >
           Mudar o Fundo
        </button>
    </div>
</template>

<script>
export default {
    name:'MudarBg',
    emit:['mudarFundo']
}
</script>