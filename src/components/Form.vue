<template>
  <div>
    <form>
      <h1>Meu form</h1>
      <br />
      <InputTxt />
      <InputTxt/>
      <InputSubmit Texto='usei props'/>
    </form>
  </div>
</template>

<script>
import InputTxt from "./form/input.vue";
import InputSubmit from "./form/submit.vue";

export default {
  name: "Form",

  components: {
    InputTxt,
    InputSubmit,
  },
};
</script>
