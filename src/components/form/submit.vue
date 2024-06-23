<template>
  <div>
    <input type="submit" :value="Texto" />
  </div>
</template>

<script>
export default {
  name: "InputSubmit",
  props:{
    Texto:String
  }
};
</script>
