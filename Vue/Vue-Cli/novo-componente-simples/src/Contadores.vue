<template>
  <div class="Contadores">
    <h2>{{ nome }}:</h2>
    <contador v-for="c in 5" :key="c" />
  </div>
</template>

<script>
import contador from "./Contador.vue";
export default {
  name: "contadores",
  data: function() {
    return {
      nome: "Contadores"
    };
  },
  components: {
    contador
  }
};
</script>